namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end
  
  desc 'outputs hola to the terminal'
  task :hola do
    puts 'hola de Rake!'
  end
end

namespace :db do
  desc 'invokes the :environment task'
  task :migrate => :environment do
    Student.create_table
  end
  
  desc 'create the students table'
  task :environment do
  require_relative './config/environment'
  end
  
  desc 'seeds the database'
  task :seed do
    require_relative './db/seeds.rb'
  end
end