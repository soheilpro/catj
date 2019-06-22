# catj
Displays JSON files in a flat format.

Input:

```
{
  "mappings": {
    "templates": [
      {
        "fields": {
          "mapping": {
            "norms": false,
            "type": "text",
            "fields": {
              "keyword": {
                "ignore_above": 256,
                "type": "keyword"
              }
            }
          }
        }
      }
    ]
  }
}
```

Output:

```
.mappings.templates[0].fields.mapping.norms = false
.mappings.templates[0].fields.mapping.type = "text"
.mappings.templates[0].fields.mapping.fields.keyword.ignore_above = 256
.mappings.templates[0].fields.mapping.fields.keyword.type = "keyword"
```

## Why?

- It makes it easier to understand the structure of JSON files.
- The output is valid JavaScript which can be used directly in code.
- It's very helpful when writing queries for tools like [jq](https://stedolan.github.io/jq/manual/).

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
