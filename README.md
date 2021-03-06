# Pupmin

Pupmin is a toolkit and utility collection for working with a Puppet cluster. Most options will require a working PuppetDB server. This gem isn't meant to replace or be an alternative to other Puppet/PuppetDB gems, but rather just serve to be a shortcut and interface into some common administrative and management tasks.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'pupmin'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install pupmin

## Usage

### In Script/Application

Include the gem, then set the configuration before calling any of the classes/methods. At minimum, you need the PuppetDB server that you'll query:

```ruby
Pupmin.configure({:puppetdb_url => 'http://puppetdb.yourdomain.tld:8080'})
```
The PuppetDB class essentially just wraps the [VoxPupuli PuppetDB Gem](https://github.com/voxpupuli/puppetdb-ruby), so the same configuration block for SSL connections can be used here.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
