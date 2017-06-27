## Sensu-Plugins-geckoboard

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-geckoboard.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-geckoboard)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-geckoboard.svg)](http://badge.fury.io/rb/sensu-plugins-geckoboard)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-geckoboard/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-geckoboard)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-geckoboard/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-geckoboard)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-geckoboard.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-geckoboard)

## Functionality

## Files
 * bin/metrics-geckoboard-push.rb

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

[Installation and Setup](http://sensu-plugins.io/docs/installation_instructions.html)

## Notes
