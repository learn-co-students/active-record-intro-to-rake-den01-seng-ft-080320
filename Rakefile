desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end


namespace :greeting do 
  desc 'outputs hello to the terminal'
  task :hello do 
    puts "hello from Rake!"
  end

  desc 'outputs holla ot the terminal'
  task :hola do 
    puts "hola de Rake!"
  end
end

desc 'drop inot the Pry console'
task :console => :environment do 
  Pry.start
end



namespace :db do 
  desc 'migrate changes to the database'
  task :migrate => :environment do 
    Student.create_table
  end

  task :environment do 
    require_relative './config/environment'
  end

  desc 'seeds the database with some dummy data'
  task :seed do 
    require_relative './db/seeds'
  end
end