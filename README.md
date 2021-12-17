# ProcessWire “Regular” site installation profile

## A Uikit v3 based blog site using Markup Regions

The front-end of this profile uses the [Uikit 3](https://getuikit.com/) 
library and includes a library of time-saving functions for working 
with Uikit 3. It stays with the default Uikit styles and we've tried 
to keep it as generic “Uikit” look as possible. That way, when someone 
wants to use it to build a site, there is very little they have to 
reverse engineer or remove. It also means that you should be able to 
plug in any Uikit 3 theme and have everything adjust perfectly to that 
theme. We currently have no theme being applied, so you just see the 
generic Uikit output.

[Live example](https://demo.processwire.com/regular/)

## Highlights

- This profile includes a [blog component](http://demo.processwire.com/regular/blog/) 
  and demonstrates how to build a simple blog in ProcessWire.

- The profile uses [Markup Regions](https://processwire.com/docs/front-end/output/markup-regions/) 
  and the ProcessWire [Functions API](https://processwire.com/api/ref/functions/#pwapi-methods-Functions-API).

- It uses the new Uikit 3 on the front-end in template files and includes 
  a handy PHP library of Uikit-specific functions.

- One of the template files (`basic-page-edit.php`) demonstrates how to 
  implement front-end editing features. When logged in (and page is 
  editable) you can edit any pages using that template on the front-end.

- Uses pagination (after 10+ blog posts) and demonstrates use of comments 
  as well. Includes a `ukPagination()` function which tailors ProcessWire's 
  MarkupPagerNav module to deliver Uikit pagination.

- Demonstrates use of a Page reference field, as used by 
[categories](http://demo.processwire.com/regular/categories/) 
in the blog. 

- The template files are easy-to-read and modify, and serve as a good 
  platform to build from. Use of Markup Regions makes them simple to 
  follow in the same way that template files using direct output tend 
  to be simple to follow.

- Demonstrates implementation of a custom hook function (see in the 
  `/site/ready.php` file).
  
## Uikit v3 functions library 

This site profile also includes a Uikit 3 PHP function library that 
simplifies some of the more verbose bits of markup you might need when 
using Uikit 3 with ProcessWire. For instance, creating a recursive 
navigation tree using uk-nav, generating a uk-navbar with dropdowns, 
rendering uk-pagination, or any number of other things. We find it 
helpful to have a few helper functions to avoid markup redundancy in 
multiple template files.

You'll see this library included with the site profile, even though 
it doesn't itself need to use all of the functions that are included. 

## To install

Depending on your version of ProcessWire, you may already have this site profile
included with the core, in which case you do not need to download it. If you find
that you do not already have it, follow the instructions below: 

- To use this site profile, you must first have a copy of ProcessWire that has 
  not yet gone through the installation process. 

- Copy the files from this repository into a `/site-regular/` directory in your
  web root (or wherever ProcessWire’s `install.php` file is located). 

- Open the URL where you've copied ProcessWire's files to in your web browser. 
  The installer should start, and when it asks you what site profile you want to
  install, you should see this profile there. Select it and continue installation.


