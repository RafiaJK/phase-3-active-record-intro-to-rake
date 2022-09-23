desc 'drop into the Pry console'
task console: :environment do
  Pry.start
end


task :environment do
  require_relative './config/environment'
end

namespace :greeting do
  desc 'outputs hello to the terminal'
    task :hello do
      puts "hello from Rake!"
    end
  
    desc 'outputs hola to the terminal'
    task :hola do
      puts "hola de Rake!"
    end
  end

namespace :greetings do
  desc 'some greeting in english'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'description of class activities'
  task :flatiron_greeting do
    puts "welcome to day 5 of ruby. it's raking time baby"
  end
end

namespace :db do
  desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end

  desc 'run the seed file'
  task seed: :environment do
    require_relative './db/seeds'
  end

end

