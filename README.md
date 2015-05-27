# catj
Displays JSON files in flat format. Handy when you need to find the full path of a node.

Input:

```
{
  "movie": {
    "name": "Interstellar",
    "year": 2014,
    "is_released": true,
    "director": "Christopher Nolan",
    "cast": [
      "Matthew McConaughey",
      "Anne Hathaway",
      "Jessica Chastain",
      "Bill Irwin",
      "Ellen Burstyn",
      "Michael Caine"
    ]
  }
}
```

Output:

```
.movie.name = "Interstellar"
.movie.year = 2014
.movie.is_released = true
.movie.director = "Christopher Nolan"
.movie.cast[0] = "Matthew McConaughey"
.movie.cast[1] = "Anne Hathaway"
.movie.cast[2] = "Jessica Chastain"
.movie.cast[3] = "Bill Irwin"
.movie.cast[4] = "Ellen Burstyn"
.movie.cast[5] = "Michael Caine"
```

## Install

```
npm install -g catj
```

## Usage

```
catj [file]
```

If no file is specified, catj reads from the standard input.

## Version History
+ **1.0**
	+ Initial release.

## Author
**Soheil Rashidi**

+ http://soheilrashidi.com
+ http://twitter.com/soheilpro
+ http://github.com/soheilpro

## Copyright and License
Copyright 2014 Soheil Rashidi

Licensed under the The MIT License (the "License");
you may not use this work except in compliance with the License.
You may obtain a copy of the License in the LICENSE file, or at:

http://www.opensource.org/licenses/mit-license.php

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
