spring = proc do
  gem 'spring'
  gem 'spring-commands-rspec'
end

rails_4 = proc do
  instance_eval(&spring)
  gem 'uglifier', '>= 1.3.0'
  gem 'coffee-rails', '~> 4.0.0'
  gem 'jquery-rails'
  gem 'turbolinks'
  gem 'sdoc'
  gem 'activeresource', '4.0.0'
  gem 'rspec-rails', '~> 3.0.1'
  # Test suite makes heavy use of attr_accessible
  gem 'protected_attributes'
  gem 'minitest-reporters'
end

#---

appraise '4.0.0' do
  instance_eval(&rails_4)
  gem 'rails', '4.0.0'
  gem 'jbuilder', '~> 1.2'
  gem 'sass-rails', '~> 4.0.0'
  gem 'bcrypt-ruby', '~> 3.0.0'
end

appraise '4.0.1' do
  instance_eval(&rails_4)
  gem 'rails', '4.0.1'
  gem 'jbuilder', '~> 1.2'
  gem 'sass-rails', '~> 4.0.0'
  gem 'bcrypt-ruby', '~> 3.1.2'
  gem 'rspec-rails', '2.99.0'
end

appraise '4.1' do
  instance_eval(&rails_4)
  gem 'rails', '~> 4.1.0'
  gem 'jbuilder', '~> 2.0'
  gem 'sass-rails', '~> 4.0.3'
  gem 'sdoc', '~> 0.4.0'
  gem 'bcrypt', '~> 3.1.7'
  gem 'protected_attributes', "~> 1.0.6"
  gem 'spring'
end

appraise '4.2' do
  instance_eval(&rails_4)
  gem 'rails', '~> 4.2.0'
  gem 'sass-rails', '~> 5.0'
  gem 'coffee-rails', '~> 4.1.0'
  gem 'jbuilder', '~> 2.0'
  gem 'sdoc', '~> 0.4.0'
  gem 'bcrypt', '~> 3.1.7'
  gem 'spring'
  gem 'protected_attributes', "~> 1.0.6"
end
