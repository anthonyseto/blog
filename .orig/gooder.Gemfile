source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

ruby '2.5.8'
# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 5.2.4', '>= 5.2.4.3'
# Use sqlite3 as the database for Active Record

#Use bcrypt for password on user ActiveModel
gem 'bcrypt', '~> 3.1.7'

#Use pagination gem for articles indexing
gem 'will_paginate', '~> 3.2'
gem 'bootstrap-will_paginate', '1.0.0'
# Use Puma as the app server
gem 'puma', '~> 3.12', '>= 3.12.4'
# Use SCSS for stylesheets
gem 'bootstrap-sass', '~> 3.4.0'
gem 'jquery-rails', '>= 4.4.0'
gem 'sass-rails', '~> 5.1', '>= 5.1.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'
# See https://github.com/rails/execjs#readme for more supported runtimes
gem 'therubyracer'
gem 'execjs'

#Use simplecov gem for generating sonarwube coverage report
gem 'simplecov', '>= 0.17.1', require: false, group: :test

# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.2', '>= 4.2.2'
# Turbolinks makes navigating your web application faster. Read more: https://github.com/turbolinks/turbolinks
gem 'turbolinks', '~> 5'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.9', '>= 2.9.1'

# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

#gem for assert_tempalte testing in Integration Test
gem 'rails-controller-testing', '>= 1.0.4'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'sqlite3'
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
  # Adds support for Capybara system testing and selenium driver
  gem 'capybara', '~> 2.18', '>= 2.18.0'
  gem 'selenium-webdriver', '>= 3.142.3'
  gem 'minitest-reporters'
end

group :development do
  # Access an IRB console on exception pages or by using <%= console %> anywhere in the code.
  gem 'web-console', '>= 3.7.0'
  gem 'listen', '>= 3.0.5', '< 3.2'
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
end

group :production do
  #since heroku production uses only postgres sql and not sqlite3
  gem 'pg'
  gem 'rails_12factor'
  # Use Redis adapter to run Action Cable in production
  gem 'redis', '~> 4.0'
end

