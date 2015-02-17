task default: :build
task travis: :build

# Add sass load paths here.
load_paths = %w(
)

# Automatically add bower_components to the load path.
load_paths << 'bower_components' if Dir.exist? 'bower_components'

# Convert list to sass arguments.
load_paths.map! { |v| ['--load-path', v] }.flatten!

# Spawn a server and kill it gracefully when interrupt is received
def spawn *cmd
  pid = Process.spawn(*cmd)

  switch = true
  Signal.trap 'SIGINT' do
    Process.kill( :QUIT, pid ) && Process.wait
    switch = false
  end
  while switch do sleep 1 end
end

desc 'Compile Sass to CSS'
task :build do
  sh 'bundle', 'exec', 'sass',
     '--update', 'stylesheets:build',
     *load_paths
end

desc 'Have Sass watch for changes'
task :watch do
  spawn 'bundle', 'exec', 'sass',
        '--watch', 'stylesheets:build',
        *load_paths
end

desc 'Remove build directory'
task :clean do
  FileUtils.remove_entry_secure 'build' if Dir.exist? 'build'
end
