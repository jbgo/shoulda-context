require 'bundler'
require 'rake'
require 'rake/testtask'

Bundler::GemHelper.install_tasks

$LOAD_PATH.unshift("lib")
load 'tasks/shoulda.rake'

Rake::TestTask.new do |t|
  t.libs << 'lib' << 'test'
  t.pattern = 'test/**/*_test.rb'
  t.verbose = false
end

desc 'Default: run tests'
task :default => [:test]
