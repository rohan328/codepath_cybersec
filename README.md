# Project 7 - WordPress Pentesting

Time spent: **5** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

### 1. (Required) Stored XSS
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [x] GIF Walkthrough: <a href="exploit1.gif">exploit1.gif</a>
  - [x] Steps to recreate: Copy the code from <a href="exploit1.txt">exploit1.txt</a> to comment field on wordpress
  
### 2. (Required) Authenticated XSS via media file metadata
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.7.3
  - [x] GIF Walkthrough: <a href="exploit2.gif">exploit2.gif</a>
  - [x] Steps to recreate: Upload a media file and add metadata using admin panel("filename <script>alert("ABC");</script>"). Access image to execute XSS.

### 3. (Required) Wordpress Large File Upload
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.15
  - [x] GIF Walkthrough: <a href="exploit3.gif">exploit3.gif</a>
  - [x] Steps to recreate: Create a large file(greater than 20mb) and add XSS script to its name. Upload it using admin portal. File wont upload but XSS will execute.

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## License

    Copyright 2020 Rohan Ohlan

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
