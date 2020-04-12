# Web-Security-Weeks-7-8-Project-WordPress-vs.-Kali
Weeks 7 &amp; 8 Project: WordPress vs. Kali

# Project 7 - WordPress Pentesting

Time spent: **6** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1.3.7-4.4 Authenticated Cross-Site Scripting (XSS) CVE-2016-1564 
  - [ 1] Summary: 
    - Vulnerability types: 3.7-4.4	
    - Tested in version: 4.2
    - Fixed in version: 4.26
  - [1 ] GIF Walkthrough: ![reply](https://user-images.githubusercontent.com/55426354/79058665-d1ece000-7c3e-11ea-992d-961c92d0f2e7.gif)
  - [ 1] Steps to recreate: Post the following XSS code into a comment or post than do->
	 <span>[http://codepath.org//<svg onload=alert('got_you')]</span>
  - [ ] Affected source code: 
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. 2.5-4.6 - Authenticated Stored Cross-Site Scripting via Image Filename CVE-2016-7168 
    - Vulnerability types:
    - Tested in version: 2.5-4.6
    - Fixed in version: 4.2
  - [ ] GIF Walkthrough: ![picture](https://user-images.githubusercontent.com/55426354/79058836-d1eddf80-7c40-11ea-972c-f45bbde089b9.gif)
  - [ ] Steps to recreate:  <ol>
<li>find an image and upload.</li>
  <li>Change the .jpg with the following script hope<img src= picture onerror =alert("picture_got_u")>.jpg</li>
<li>Create new media in library and upload the image.</li>
<li>View attachment page to view the image post.</li>
</ol>
<hr>
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
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

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.