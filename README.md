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
Examples:
	omnavi # read from standard input
	omanvi -f example-input-file.txt # read from specified file instead of stdin
	omnavi -f example-input-file.txt -d 'yesterday 10:40am UTC' # also use date
	omnavi -d 'last wednesday' # read from standard input, but also compare against specified date
```

# DEPENDENCIES

* GNU coreutils
* GNU sed
* curl
* youtube-dl
* jq

