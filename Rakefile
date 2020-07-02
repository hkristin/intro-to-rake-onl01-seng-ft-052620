require 'pry'

task :environment do
  require_relative './config/environment'
end

desc 'outputs hello to the terminal'
namespace :greeting do 
  task:hello do
      puts "hello from Rake!"
    end
    
desc 'outputs hola to the terminal'
  task:hola do
       puts "hola de Rake!"
  end  
 
namespace :db do
  desc 'migrate changes to your database'
    migrate:environment do
    Student.create_table
  end

  desc 'seed the database with some dummy data'
    db:seed do
    require_relative './db/seeds.rb'
  end

desc 'drop into the Pry console'
  console:environment do
  Pry.start
end
end
end
