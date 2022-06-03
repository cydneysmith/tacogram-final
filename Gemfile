source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "2.7.6"

#if not in a group, all these guys get installed into all our environments
gem "rails", "~> 7.0.2.2"

gem "puma", "~> 5.0"
gem "bcrypt", "~> 3.1.7"
gem "tzinfo-data", platforms: %i[ mingw mswin x64_mingw jruby ]
# gem "aws-sdk-s3", require: false

group :development, :test do
  gem "debug", platforms: %i[ mri mingw x64_mingw ]
end

group :development do
  gem "tabulo"
  gem "web-console"
  gem "sqlite3", "~> 1.4"
end

#I want this installed only in the production enviro
group :production do
  gem "pg" #ruby interface to postgresql system
end

