# Track Duration

This is a gem to handle time duration, parsing a string to seconds and vice-versa.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'track_duration'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install track_duration

## Usage

### Informing a string and converting to the number of seconds

```ruby
require 'track_duration'

# 3 minutes and 45 seconds
> puts TrackDuration.new('3:45').seconds
225

> puts TrackDuration.new('15:03:45').seconds
54225

> puts TrackDuration.new('63:03:45').seconds
227025
```

### Informing the number of seconds and converting to a string
```ruby
require 'track_duration'

> puts TrackDuration.new(225).to_s
03:45

> puts TrackDuration.new(54_225).to_s
15:03:45

> puts TrackDuration.new(227_025).to_s
63:03:45
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/rodrigovdb/duration. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/rodrigovdb/duration/blob/master/CODE_OF_CONDUCT.md).

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Track Duration project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/rodrigovdb/duration/blob/master/CODE_OF_CONDUCT.md).
