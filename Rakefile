# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require File.expand_path('../config/application', __FILE__)

Rails.application.load_tasks



# bin/rake crash => SEGFAULT
# DISABLE_SPRING=true bin/rake crash => nothing
task crash: :environment do
  r = Typhoeus::Request.new("https://www.google.com", method: :get)
  r.run
end
