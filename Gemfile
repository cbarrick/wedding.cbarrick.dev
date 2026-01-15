source "https://rubygems.org"

gem "logger"

# We use Jekyll to build the site.
gem "jekyll", "~> 4.4.0"

# Add Jekyll plugins to this group.
group :jekyll_plugins do
    gem "jekyll-default-layout"
    gem "jekyll-sass-converter"
    gem "jekyll-seo-tag"
end

# Enables `jekyll serve`.
# Not included (or needed) by GitHub Pages.
gem "webrick", "~> 1.7"

# Windows and JRuby do not include zoneinfo files,
# so bundle the tzinfo-data gem and associated library.
platforms :windows, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.0", :install_if => Gem.win_platform?

# kramdown v2 ships without the gfm parser by default.
gem "kramdown-parser-gfm"

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds
# since newer versions of the gem do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
