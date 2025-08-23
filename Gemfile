source "https://rubygems.org"

ruby "3.2.5"

# Rails framework
gem "rails", "~> 7.1.0"

# Database
gem "sqlite3", "~> 1.6.0"

# Web server
gem "puma", "~> 6.0"

# Asset pipeline
gem "sprockets-rails"

# JavaScript
gem "importmap-rails"
gem "turbo-rails"
gem "stimulus-rails"

# JSON API
gem "jbuilder"

# Windows compatibility
gem "tzinfo-data", platforms: %i[ mingw mswin x64_mingw jruby ]

group :development, :test do
  # Testing
  gem "minitest-reporters", "~> 1.6"
  gem "guard"
  gem "guard-minitest"
end

group :development do
  # Debugging
  gem "debug", platforms: %i[ mri mingw mswin x64_mingw ]
  
  # Console
  gem "web-console"
end

group :test do
  # System testing
  gem "capybara", "~> 3.40"
  gem "selenium-webdriver", "~> 4.10"
end
