source "http://rubygems.org"
gemspec

gem "rake"

git "git://github.com/rails/rails.git" do
  gem "activemodel"
end

platforms :mri_19 do
  unless ENV["CI"]
    gem "debugger"
  end
end

group :test do
  gem "rspec", "~> 2.11"

  unless ENV["CI"]
    gem "guard"
    gem "guard-rspec"
    gem "rb-fsevent"
  end
end
