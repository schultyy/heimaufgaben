---
title: Phonebook
---

# Phonebook

## Technologies

- JSON

## Description

Write a command line program which can resolve names and phone numbers based on a `phonebook.json` file.
The program asks the user to enter either a name or a phone number. It then tries to resolve the person. If it fails, it should print
an error that no such person exists.

```bash
$ ruby phonebook.rb "Franz Mueller"
> 543534534 

$ ruby phonebook.rb 78612
> Lisbeth Maier

$ ruby phonebook.rb "Max Muetze"
> Person not found
```

The `phonebook.json` looks like this:

```json
[
  {
    "name": "Franz Mueller",
    "phone": "543534534"
  },
  {
    "name": "Josef Schneider",
    "phone": "8632"
  },
  {
    "name": "Lisbeth Maier",
    "phone": "78612"
  },
  {
    "name": "Edit Muetze",
    "phone": "538921"
  }
]
```

`phonebook.json` and `phonebook.rb` are located in the same directory. 

## Hints

### Reading JSON files

```ruby
require 'json'

contents = JSON.parse(File.read('phonebook.json'))
# contents then returns an array of hashes
# A single hash represents an entry in the phonebook
```

### Get commandline arguments

Get commandline arguments like this:

```ruby
puts "ARGS: #{ARGV.inspect}"
```
