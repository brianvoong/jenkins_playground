# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.


require 'ci/reporter/rake/rspec'
task :rspec => 'ci:setup:rspec'

require File.expand_path('../config/application', __FILE__)

JenkinsPlayground::Application.load_tasks

task :dowork do
  ruby "spec/controllers/widgets_controller_spec.rb"
end