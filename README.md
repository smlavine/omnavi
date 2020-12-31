# OMNAVI

```
omnavi - A program to receive YouTube subscriptions without a Google account.
Copyright (C) 2020 Sebastian LaVine <mail@smlavine.com>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see http://www.gnu.org/licenses/.

Usage: omnavi [-hn] [-d date] [-f file]
Options:
	-h          Print this help and exit.
	-n          Don't print Unicode line characters when formatting.
	-d date     Instead of comparing against 24 hours ago,
	            compare against this date.
	-f file     Instead of reading from stdin, read from this file.
	-g video    Print the channel ID of the uploader of the given video.
```

# EXAMPLES

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

# DEPENDENCIES

* GNU coreutils
* GNU bash
* GNU sed
* curl
* youtube-dl
* jq

