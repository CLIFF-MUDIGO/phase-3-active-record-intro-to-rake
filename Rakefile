namespace :greeting do
  desc "Prints 'hello from Rake!'"
  task :hello do
    puts "hello from Rake!"
  end
end

namespace :greeting do
  desc "Prints 'hola de Rake!'"
  task :hola do
    puts "hola de Rake!"
  end
end

task :console do
  exec "pry -r ./config/environment.rb"
end
task :environment do
  require_relative 'config/environment'
end

namespace :db do
  desc "Run database migrations"
  task :migrate => :environment do
  
  end
end
namespace :db do

  desc 'seed the database with some dummy data'
  task seed: :environment do
    require_relative './db/seeds'
  end
end