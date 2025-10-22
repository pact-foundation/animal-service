source 'https://rubygems.org'

group :development, :test do
  gem 'rspec'
  gem 'pry'

  if ENV['X_PACT_DEVELOPMENT']
    gem 'pact', path: '../pact-ruby'
  else
    gem 'pact'
  end
  group :v2, optional: true do
    gem "pact-ffi", "~> 0.4.28"
    gem 'combustion'
    gem 'webmock'
    gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw]  
  end
end

gem 'rake'
gem 'rack'
gem 'json'
if Gem.win_platform?
  gem 'sqlite3', force_ruby_platform: true
else
  gem 'sqlite3'
end
gem 'sequel'
gem 'sinatra'
