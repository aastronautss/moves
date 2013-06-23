# Moves

Ruby client for [Moves](http://www.moves-app.com/)

## Usage

Create a client.

```ruby
client = Moves::Client.new(access_token)
```

Get profile

```ruby
client.profile
```

Get daily summary

```ruby
client.daily_summary # default to current day
client.daily_summary(:from => "2013-06-20", :to => "2013-06-23") # max 31 days
```

Get daily activities

```ruby
client.daily_activities # default to current day
client.daily_activities(:from => "2013-06-20", :to => "2013-06-23") # max 7 days
```

Get daily places

```ruby
client.daily_places # default to current day
client.daily_places(:from => "2013-06-20", :to => "2013-06-23") # max 7 days
```

Get daily storyline

```ruby
client.daily_storyline # default to current day
client.daily_storyline(:from => "2013-06-20", :to => "2013-06-23") # max 7 days
```

## Installation

Add this line to your application's Gemfile:

```ruby
gem "moves"
```

And then execute:

```sh
bundle
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
