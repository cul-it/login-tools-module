# login-tools-module

Provides a block with a link to the login page, including a &destination= parameter 
that returns the user to the original page after login.

How to set up forms with login required

* limit the webform's Submission Access to authenticated user ( Webform > Form settings )
* place the block 'Login Tools - require login to view a form' on the page where the form is
* configure the String Overrides module to remove the 'login' link from the warning message Drupal places on the form

```
ORIGINAL:
You must <a href="!login">login</a> to view this form.
REPLACEMENT:
You must login to view this form.
```