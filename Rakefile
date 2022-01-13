task :environment do
  require_relative './config/environment'
end

namespace :greeting do
desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

desc "outputs hola to the terminal"
task :hola do
  puts "hola de Rake!"
end
end

namespace :farewell do
desc "outputs goodbye to the terminal"
task :goodbye do
  puts "goodbye from Rake!"
end

desc "outputs nos vemos to the terminal"
task :nosvemos do 
  puts "nos vemos from Rake!"
end
end

namespace :db do
  desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end
  desc 'seed the databse with some dummy data'
  task seed: :environment do 
    require_relative './db/seeds'
  end
end

desc 'drop into the Pry console'
task console: :environment do
  Pry.start
end