source 'https://rubygems.org'

group :rake do
  puppetversion = ENV.key?('PUPPET_VERSION') ? "#{ENV['PUPPET_VERSION']}" : ['>= 3.0.0','< 5.0']
  gem 'puppet', puppetversion
  gem 'puppet-lint'
  gem 'puppetlabs_spec_helper', '>=0.2.0'
  gem 'rake',         '>=0.9.2.2'
  gem 'rspec-system-puppet',     :require => false
  gem 'serverspec',              :require => false
  gem 'rspec-system-serverspec', :require => false
  gem 'librarian-puppet' , '>=2.0'
  gem 'highline'
  if RUBY_VERSION =~ /^1\.9\./ or RUBY_VERSION =~ /^1\.8\./
    gem 'json', '< 2.0' # newer versions requires at least ruby 2.0
    gem 'json_pure', '< 2.0.0'
    gem 'fog-google', '< 0.1.1'
  end
  gem 'rspec-puppet'
  gem 'parallel_tests'
end

group :development do
  gem 'puppet-blacksmith',  '~> 3.0'
  gem 'metadata-json-lint',      :require => false
  gem 'travis'
  gem 'travis-lint'
  gem 'rubocop'
end
