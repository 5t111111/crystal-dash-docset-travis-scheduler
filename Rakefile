require 'travis'

desc 'call travis to build restart'
task :default do
  Travis.access_token = ENV['TRAVIS_ACCESS_TOKEN']
  repository = Travis::Repository.find('5t111111/crystal-dash-docset')
  repository.last_build.restart
end
