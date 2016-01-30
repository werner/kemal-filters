# kemal-filters

Filters callback, similar to sinatra: http://www.sinatrarb.com/intro.html#Filters

## Installation


Add this to your application's `shard.yml`:

```yaml
dependencies:
  kemal-filters:
    github: werner/kemal-filters
```


## Usage

```crystal
  require "kemal"
  require "kemal-filters"

  add_filters

  before "/home" do |env|
    env.redirect "/other"
  end

  get "/home" do
    "Hello World"
  end

  get "/other" do
    "Other Page"
  end
```

## Development

TODO: Write development instructions here

## Contributing

1. Fork it ( https://github.com/werner/kemal-filters/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create a new Pull Request

## Contributors

- [werner](https://github.com/werner) Werner - creator, maintainer
