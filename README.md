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

Usage: omnavi [-h] [-f file] [-d date]
Options:
-h          Prints this help.
-f file     Instead of reading from stdin, reads from this file.
-d date     Instead of comparing against 24 hours ago,
            compares against this date.
Examples:
omnavi  # reads from standard input
omanvi -f feeds.txt  # reads feeds from feeds.txt
omnavi -f feeds.txt -d 'yesterday 10:40am UTC'  # also uses specified date
omnavi -d 'last wednesday'  # reads from standard input, but also compares against specified date
```

# DEPENDENCIES
* GNU coreutils
* GNU sed
* curl
* youtube-dl
* jq

