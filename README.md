# Hipster Lorem :tophat:

This is a super duper insanely simplistic gem that generates hipster lorem ipsum for no reason at all. Wee! Just a learning exercise for me to learn what creating gems is all about.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'lorem'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install lorem

## Usage

Just install (except you can't because it's local... :smile:), and bam - You have hipster lorem sentences at your fingertips just by calling:

```ruby
Lorem.ipsum
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/amlydu/lorem.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

## self.notes

Used this [RailsCast](http://railscasts.com/episodes/245-new-gem-with-bundler) tutorial to learn moar about creating a gem with bundler.

### Bash commands used in the tutorial:

```
$ bundle gem lorem
$ gem build lorem.gemspec
$ gem push lorem-0.0.1.gem
$ bundle
$ rake -T
$ rake build
$ rake install
$ rake release
```
- The `gem build gem_name.gemspec` generates a new file `gem_name-version_number.gem`
- Pushing the file pushes it to rubygems.org and publishes it for all the :earth_americas: to use
- The `bundle gem lorem` assumes that you're using git; intializes a git repo
- `gemspec` file is the :heart: of the gem
  - File attributes are determined at runtime - automatically inherits behavior from the `.gitignore` file
  - Loading version file constant from `lib/your_gem/version.rb`
    - Change this value and republish gem when you're changing versions

