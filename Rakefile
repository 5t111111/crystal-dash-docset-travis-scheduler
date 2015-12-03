require 'travis'

desc 'call travis to build restart'
task :run_travis_build do
  Travis.access_token = ENV['TRAVIS_TOKEN']
  repository = Travis::Repository.find('5t111111/crystal-dash-docset')
  repository.last_build.restart
end
