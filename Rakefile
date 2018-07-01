
namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola, en espanol!'
  task :hola do
    puts "Hola, como estas?"
  end
end

namespace :db do
  desc 'migrate changes to the database'
  task :migrate => :environment do
    Student.create_table
  end
end

task :environment do 
  require_relative './config/environment'
end 
