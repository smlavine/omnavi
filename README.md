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
    omnavi # reads from standard input
    omanvi -f feeds.txt # reads feeds from feeds.txt
    omnavi -f feeds.txt -d 'yesterday 10:40am UTC' # also uses specified date
    omnavi -d 'last wednesday' # reads from standard input, but also compares against specified date
Input format:
    <channel-id>            	<Only the first column of input is read.>
    ...
    UCL7DDQWP6x7wy0O6L5ZIgxg	2ndJerma
    UC9_p50tH3WmMslWRWKnM7dQ	Adam Ragusea
    UCBa659QWEk1AI4Tg--mrJ2A	Tom Scott
    UCBgWgQyEb5eTzvh4lLcuipQ	Wikitongues

```

# DEPENDENCIES

* GNU coreutils
* GNU sed
* curl
* youtube-dl
* jq

