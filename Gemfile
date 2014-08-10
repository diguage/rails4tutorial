source 'https://ruby.taobao.org/'
# source 'https://rubygems.org'

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '4.1.4'
# Use SCSS for stylesheets
gem 'sass-rails', '~> 4.0.3'
# Use Uglifier as compressor for JavaScript assets
# gem 'uglifier', '>= 1.3.0' # Rails 模板中所用版本
gem 'uglifier', '~> 2.5.3'
# Use CoffeeScript for .js.coffee assets and views
# gem 'coffee-rails', '~> 4.0.0' # Rails 模板中所用版本
gem 'coffee-rails', '~> 4.0.1'
# See https://github.com/sstephenson/execjs#readme for more supported runtimes
# gem 'therubyracer',  platforms: :ruby

# Use jquery as the JavaScript library
gem 'jquery-rails', '~> 3.1.1'
# Turbolinks makes following links in your web application faster. Read more: https://github.com/rails/turbolinks
gem 'turbolinks', '~> 2.2.2'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
# gem 'jbuilder', '~> 2.0' # Rails 模板中所用版本
gem 'jbuilder', '~> 2.1.3'
# bundle exec rake doc:rails generates the API under doc/api.
group :doc do
  gem 'sdoc', '~> 0.4.0', require: false
end

# Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
gem 'spring', '~> 1.1.3',        group: :development

# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use unicorn as the app server
# gem 'unicorn'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

# Use debugger
# gem 'debugger', group: [:development, :test]

group :development, :test do
  # Use sqlite3 as the database for Active Record
  gem 'sqlite3', '~> 1.3.9'
  # gem 'rspec-rails', '2.13.1'  # 书中所用版本，以下相同，不再赘述。
  #gem 'rspec-rails', '~> 3.0.2'
  gem 'rspec-rails', '~> 2.14.2'
  # gem 'guard-rspec', '2.5.0'
  gem 'guard-rspec', '~> 4.3.1'
  gem 'spork-rails', '4.0.0'
  # gem 'guard-spork', '1.5.0'
  gem 'guard-spork', '~> 1.5.1'
  # gem 'childprocess', '0.3.6'
  gem 'childprocess', '~> 0.5.3'
end

group :test do
  # gem 'selenium-webdriver', '2.35.1'
  gem 'selenium-webdriver', '~> 2.42.0'
  # gem 'capybara', '2.1.0'
  gem 'capybara', '~> 2.4.1'

  # 根据系统类型，自动选择合适的Gem；或者使用下面的手动选择Gem
  if RbConfig::CONFIG['target_os'] =~ /mswin|mingw/i  #Windows?
    gem 'rb-notifu', '0.0.4'
    gem 'win32console', '1.3.2'
    gem 'wdm', '0.1.0'
  elsif RbConfig::CONFIG['target_os'] =~ /linux|unix|freebsd|openbsd|netbsd/i  #Linux?
    # # gem 'libnotify', '0.8.0'
    gem 'libnotify', '~> 0.8.3'
  else   #Mac?
    gem 'growl', '1.0.3'
  end
end

group :production do
  # gem 'pg', '0.15.1'
  gem 'pg', '~> 0.17.1'
end
