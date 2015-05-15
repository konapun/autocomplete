# autocomplete
Get autocompletion suggestions

## Usage
```ruby
ac = Autocomplete.new(['can', 'Canada', 'soda', 'sock', 'song', 'sound', 'sand', 'zebra'])

# By default, suggestions are case-sensitive. Make results case-insentitive by:
ac.case_sensitive = false

ca = ac.autocomplete('ca') #  => ['can', 'Canada']
so = ac.autocomplete('so') # => ['soda', 'sock', 'song', 'sound']
s = ac.autocomplete('s') # => ['soda', 'sock', 'song', 'sound', 'sand']
```
