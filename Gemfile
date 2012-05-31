source :rubygems

# gem 'slyphon-zookeeper', :path => '~/zookeeper'

# gem 'zookeeper', :path => "~/zookeeper"

# this is the last known commit that we tested against and is passing.
# keep closer track of this stuff to make bisecting easier and travis more
# accurate

# git 'git://github.com/slyphon/zookeeper.git', :tag => 'dev/zk/00006' do
#   gem 'zookeeper', '~> 1.1.0'
# end

gem 'rake', :group => [:development, :test]
gem 'pry',  :group => [:development]

group :docs do
  gem 'yard', '~> 0.8.0'

  platform :mri_19 do
    gem 'redcarpet'
  end
end

platform :mri_19 do
  gem 'simplecov', :group => :coverage, :require => false
end

group :development do
  gem 'guard',          :require => false
  gem 'guard-rspec',    :require => false
  gem 'guard-shell',    :require => false
  gem 'guard-bundler',  :require => false

  if RUBY_PLATFORM =~ /darwin/i
    gem 'growl',       :require => false
    gem 'rb-readline', :platform => :ruby
  end
end

group :test do
  gem 'rspec', '~> 2.8.0'
  gem 'flexmock', '~> 0.8.10'
  gem 'zk-server', '~> 1.0.1'
end

# Specify your gem's dependencies in zk.gemspec
gemspec


# vim:ft=ruby
