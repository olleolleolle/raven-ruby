source "https://rubygems.org/"

gemspec

if ENV["RAILS_VERSION"] && (ENV["RAILS_VERSION"].to_i == 4)
  gem "rails", "< 5"
elsif ENV["RAILS_VERSION"] && (ENV["RAILS_VERSION"].to_i == 5)
  gem "rails", "< 6"
end

if RUBY_VERSION < '2.0'
  gem "mime-types", "< 3.0.0"
  gem "nokogiri", "~> 1.6.8"
  gem "rack", "~> 1.6.8"
  gem "sidekiq", "< 3.2"
else
  gem "rack"
  gem "sidekiq"
end
gem "pry"
gem "pry-coolline"
gem "benchmark-ips"
gem "benchmark-ipsa" if RUBY_VERSION > '2.0'
gem "ruby-prof", platform: :mri
gem "rake"
gem "rubocop", "~> 0.41.1"
gem "rspec"
gem "rspec-rails"
gem "timecop"
gem "test-unit", platform: :mri if RUBY_VERSION > '2.2'
