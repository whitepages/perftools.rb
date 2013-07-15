require 'pathname'
ENV['BUNDLE_GEMFILE'] ||= File.expand_path("../Gemfile", Pathname.new(__FILE__).realpath)
require 'rubygems'
require 'bundler/setup'
require 'gemtools/rake_task'

Bundler::GemHelper.install_tasks
Gemtools::RakeTask.install_tasks

Dir['tasks/**/*.rake'].each { |rake| load rake }
