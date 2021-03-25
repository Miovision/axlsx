source 'https://rubygems.org'

gem 'mimemagic', github: 'mimemagicrb/mimemagic', branch: :master, ref: 'cfb06c8bc700b7c45e069455becb7f3cb03b0b52'
gemspec

group :test do
  if RUBY_VERSION.to_i < 2
    gem 'rake', '>= 0.8.7', '< 11'
    gem 'json', '< 2'
  else
    gem 'rake'
  end
  gem 'simplecov'
  gem 'test-unit'
end

group :profile do
  gem 'ruby-prof', :platforms => :ruby
end

platforms :rbx do
  gem 'rubysl'
  gem 'rubysl-test-unit'
  gem 'racc'
  gem 'rubinius-coverage', '~> 2.0'
end
