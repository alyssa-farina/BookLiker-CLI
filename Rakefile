require_relative './config/environment'

require 'sinatra/activerecord/rake'
require 'colorize'

desc "Start our app console"
task :c do
  ActiveRecord::Base.logger = Logger.new(STDOUT)
  Pry.start
end

desc "start our app"
task :start do
  app = BookLiker.new
  app.run
end