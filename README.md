# [omnavi](https://sr.ht/~smlavine/omnavi)

A CLI YouTube subscription aggregator. It parses channel Atom feeds and
formats video info into a easy-to-read text file, all without needing a
Google account.

```
Usage: omnavi [-hn] [-d date] [-f file] [-g video]
Options:
	-h          Print this help and exit.
	-n          Don't print Unicode line characters when formatting.
	-d date     Instead of comparing against 24 hours ago,
	            compare against this date.
	-f file     Instead of reading from stdin, read from this file.
	-g video    Print the channel ID of the uploader of the given video.
```

# Examples

To read channel IDs from standard input and use the default date and formatting
settings, simply run:

```
omnavi
```

To read from a file instead of standard input:

```
omnavi -f example-input-file.txt
```

To compare against a different date than the default (24 hours ago):

```
omnavi -d 'last wednesday'
```

To get the uploader of a certain video:

```
omnavi -g https://www.youtube.com/watch?v=jNQXAC9IVRw
```

Options can be also be joined together, like so:

```
omnavi -nf example-input-file.txt -d 'April 15'
```

# Dependencies

* GNU coreutils
* GNU bash
* GNU sed
* curl
* youtube-dl
* jq

# Copyright

Copyright (C) 2020 Sebastian LaVine <mail@smlavine.com>

Licensed under the GPL, version 3 or later. See [LICENSE][license].

[license]: https://git.sr.ht/~smlavine/omnavi/tree/master/item/LICENSE
