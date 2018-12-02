desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end



namespace :db do

  desc "set up environment"
  task :environment do
    require_relative './config/environment'
  end

  desc "migrates changes to DB"
  task :migrate => :environment do
    Student.create_table
  end
  desc "create data"
  task :seed do
    require_relative './db/seeds'
  end
end

namespace :greeting do
  desc "outputs  hello"
  task :hello do
    puts "hello from Rake!"
  end
  
  desc "outputs hola"
  task :hola do
     puts "hola de Rake!"
  end

  
end

