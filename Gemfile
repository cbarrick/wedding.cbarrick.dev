source "https://rubygems.org"

# We use Jekyll to build the site.
gem "jekyll", "~> 3.10.0"

# The github-pages gem transitively depends on all of the gems available
# in the Github Pages build environment. With this, we can use any of
# the Jekyll plugins available on Github.
#
# For a full list of plugins, see <https://pages.github.com/versions/>.
gem "github-pages", group: :jekyll_plugins

# Add additional Jekyll plugins here.
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.6"
  gem "minima", "~> 2.0" # The default theme for new Jekyll sites.
end

# Enables `jekyll serve`.
# Not included (or needed) by GitHub Pages.
gem "webrick", "~> 1.7"

# Windows and JRuby do not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
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
