# reCAPTCHA for Drupal
## Important

This package is to fix Drupal 10 upgrade captcha contrib module compose 
dependencies. Once your project is already run on Drupal 10 version 
rollback to drupal/recaptcha original contrib module.

## CONTENTS OF THIS FILE

* reCAPTCHA for Drupal
* DEPENDENCIES
* CONFIGURATION
* KNOWN ISSUES

## reCAPTCHA for Drupal

The reCAPTCHA module uses the reCAPTCHA web service to improve the CAPTCHA
system and protect email addresses. For more information on what reCAPTCHA is,
please visit: [reCAPTCHA](https://www.google.com/recaptcha)

This version of the module uses the new Google No CAPTCHA reCAPTCHA API.

## DEPENDENCIES

 * The reCAPTCHA module depends on the
   [CAPTCHA module](https://drupal.org/project/captcha)


## CONFIGURATION

    1. Enable reCAPTCHA and CAPTCHA modules in: *admin/modules*

    2. You'll now find a reCAPTCHA tab in the CAPTCHA administration page
       available at: *admin/config/people/captcha/recaptcha*

    3. Register your web site [in the reCAPTCHA Administration](
       https://www.google.com/recaptcha/admin/create)

    4. Input the site and private keys into the reCAPTCHA settings

    5. Visit the Captcha administration page and set where you want the
       reCAPTCHA form to be presented: *admin/config/people/captcha*



## KNOWN ISSUES

- cURL requests fail because of outdated root certificate. The reCAPTCHA module
  may not able to connect to Google servers and fails to verify the answer.

  [See Issue #2481341](https://www.drupal.org/node/2481341) for more detail.



## THANK YOU

 * Thank you goes to the reCAPTCHA team for all their
   help, support and their amazing Captcha solution
       [recaptcha](https://www.google.com/recaptcha)
