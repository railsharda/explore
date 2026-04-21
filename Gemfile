# frozen_string_literal: true

source "https://rubygems.org"

# Jekyll is used to build the static site
gem "jekyll", "~> 3.9"

# GitHub Pages compatible plugins
gem "jekyll-feed", "~> 0.15"
gem "jekyll-sitemap", "~> 1.4"
gem "jekyll-redirect-from", "~> 0.16"

# Used for linting and validation
gem "html-proofer", "~> 4.4"

# Markdown rendering
gem "kramdown", "~> 2.4"
gem "kramdown-parser-gfm", "~> 1.1"

# Development and testing tools
group :development, :test do
  gem "rake", "~> 13.0"
  gem "rubocop", "~> 1.57"
  gem "rubocop-rake", "~> 0.6"
  # rubocop-performance helps catch slow Ruby patterns
  gem "rubocop-performance", "~> 1.19"
  # pry is handy for debugging locally
  gem "pry", "~> 0.14"
  # pry-byebug adds step-by-step debugging (next, step, continue commands)
  gem "pry-byebug", "~> 3.10"
  # awesome_print makes console output much more readable during local dev
  gem "awesome_print", "~> 1.9"
  # binding_of_caller is required by better_errors for full REPL in error pages
  gem "better_errors", "~> 2.10"
  gem "binding_of_caller", "~> 1.0"
  # solargraph provides IDE-like autocomplete and type checking in VS Code
  gem "solargraph", "~> 0.49"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", platforms: %i[mingw x64_mingw mswin]
