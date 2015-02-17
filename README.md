## Sensu-Plugins-geckoboard

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-geckoboard.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-geckoboard)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-geckoboard.svg)](http://badge.fury.io/rb/sensu-plugins-geckoboard)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-geckoboard/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-geckoboard)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-geckoboard/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-geckoboard)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-geckoboard.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-geckoboard)

## Functionality

## Files
 * bin/metrics-geckoboard-push

## Usage

```
{
 "geckoboard": {
    "checks": {
      "my.newrelic.throughput": {
        "type":"geckometer",
        "min":"200",
        "max":"40000",
        "widget_key":"12322-a831fsdda99f0jajd0fjas0dfja0fju9"
      },
      "my.newrelic.responsetime": {
        "type":"number_and_secondary_value",
        "widget_key":"12322-df2f2fw29f9jf9sdfsf02ihf020s0dhf"
      }
    },
    "api_key":"9239932fwew8f8777ff28fh8hf8dh"
 }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-geckoboard -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-geckoboard`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-geckoboard' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-geckoboard' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
