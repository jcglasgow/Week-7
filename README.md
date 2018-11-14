# Week-7
Week 7 lesson
 Project 7 - WordPress Pentesting

Time spent: 6 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. XSS for post upload
  - [ ] Summary: XSS placed in name of file uploaded to post can be triggered when viewing the attachment.
    - Vulnerability types:XSS
    - Tested in version:4.7
    - Fixed in version: Uknown
  - [ ] GIF Walkthrough: <img src="https://i.imgur.com/aDRzi0V.gifv" width="800">
  - [ ] Steps to recreate: 
        Login with post rights. Create new post. Add attachment with XSS script as file name into the body of the message.View the attachment after publication.  
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
2. Brute force authentication
  - [ ] Summary: Wordpress does not limit login attempts. Brute force thru word bank can potentially allow unauthorized access.
    - Vulnerability types: Brute Force
    - Tested in version: 4.7
    - Fixed in version: Uknown
  - [ ] GIF Walkthrough:<img src="https://i.imgur.com/NoXUdRx.gifv" width="800">
  - [ ] Steps to recreate: Locate user name. Open Burp. Copy url to Burp intruder. Load word bank and attack the designated parameter.
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
    
3. (Required) PHP script allows unauthenticated access
  - [ ] Summary: Html input shows potential of vulnerability that allows unauthenticated access to content.
    - Vulnerability types:PHP
    - Tested in version:4.7
    - Fixed in version: Unknown
  - [ ] GIF Walkthrough: <img src="https://i.imgur.com/K6tFxbG.gifv" width="800">
  - [ ] Steps to recreate: Locate host run on wordpress. Type the associated script in the html. 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).



## License

    Copyright [2018] [SupaHakaY2K]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
