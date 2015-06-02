# autocomplete
Get autocomplete suggestions for a string given an array of possible values

## Usage
```ruby
ac = Autocomplete.new(['can', 'Canada', 'soda', 'sock', 'song', 'sound', 'sand', 'zebra'])

# By default, suggestions are case-sensitive. Make results case-insentitive by:
ac.case_sensitive = false

ca = ac.autocomplete('ca') #  => ['can', 'Canada']
so = ac.autocomplete('so') # => ['soda', 'sock', 'song', 'sound']
s = ac.autocomplete('s') # => ['soda', 'sock', 'song', 'sound', 'sand']
```

If you'd like to search a corpus for a string appearing in any position, run `autocomplete` with the optional second
argument set to `true`

```ruby
ou = ac.autocomplete('ou', true) # => ['sound']
```
