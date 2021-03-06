# DevcampCopyrightViewTool

Utility for adding copyright statement from rails course.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'devcamp_copyright_view_tool'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install devcamp_copyright_view_tool

## Usage

In a controller:
```
before_action :set_copyright

def set_copyright
  @copyright = DevcampCopyrightViewTool::Renderer.copyright 'Antun Karlovac', 'All rights reserved'
end
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

Run `gem build devcamp_copyright_view_tool.gemspec` to build.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/devcamp_copyright_view_tool.


## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
