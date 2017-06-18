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


namespace :db do

  desc 'loads the environment'
  task :environment do
    require_relative './config/environment'
  end

  desc 'invokes the :environment task as a dependency'
  task :migrate => :environment do
    require_relative './config/environment'
  end

  desc 'loads dummy data from seed file'
  task :seed do
    require_relative './db/seeds'
  end

end
