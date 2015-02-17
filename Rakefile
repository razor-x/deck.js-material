task default: :build
task travis: :build

desc 'Compile Sass to CSS'
task :build do
  sh 'bundle', 'exec', 'sass', '--update', 'stylesheets:build'
end

desc 'Remove build directory'
task :clean do
  FileUtils.remove_entry_secure 'build' if Dir.exist? 'build'
end
