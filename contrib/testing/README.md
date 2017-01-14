# Testing

## Unit tests
When whackpad is not running in production, unit tests can be run by requesting `/ep/unit-tests/run`.

## Integration tests
whackpad integration tests expect a running whackpad instance on https://stage.hackpad.com.

## Dependencies
* Python
* Selenium: `pip install -U selenium`
* ImageMagick: http://www.imagemagick.org/script/binary-releases.php
* PIL: https://developers.google.com/appengine/docs/python/images/installingPIL
* Wand: `pip install Wand`

Mac users might need to export `MAGICK_HOME=/opt/local`

## Pre-requistes on website
jQuery (for sendkeys library support)

## Setup
Edit global.cfg
  - required: command_executor
  - optional: cookie_* values

## Running
./run.py

## Comparing/Saving
./compare.py

## CI
Some testing infrastructure for a CI exists in Jenkins, which should be converted to run on a 'public CI' such as Travis.
