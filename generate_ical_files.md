---
title: Generate ical file
---

# Generate ical file

## Technologies

- Bundler
- https://github.com/icalendar/icalendar

## Description

Write a commandline program that generates a new calendar event in the iCal format.
It asks the user about alle necessary fields:

```bash
$ ruby calendar_event.rb
Summary > "Buy a new cat"
Description > "Buy a new cat"
Start > 20141212
End > 20141213
Filename > new.ics
Writing to new.ics
```

## Hints

To include a third party library, you need to use a `Gemfile`:

```ruby
source 'https://rubygems.org/

gem 'icalendar'
```
