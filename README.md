# SAML Client
---------
Author: Erik Jan de Wit   
Level: Intermediate   
Technologies: Javascript, Cordova, RHMAP   
Summary: A demonstration of how to synchronize a single collection with RHMAP.   
Community Project: [Feed Henry](http://feedhenry.org)   
Target Product: RHMAP   
Product Versions: RHMAP 3.8.0+   
Source: https://github.com/feedhenry-templates/sync-cordova-app   
Prerequisites: fh-js-sdk : 3.0.+, cordova 4.0+   

## What is it?

This application shows how you can use SAML with the RHMAP platform, it should be used in combination with the [SAML service](https://github.com/feedhenry-templates/saml-service) and the [SAML could app](https://github.com/feedhenry-templates/saml-cloud-app) have a look at the [notes](https://github.com/feedhenry-templates/saml-service/blob/master/NOTES.md) how to setup the service.  Refer to [fhconfig.json](www/fhconfig.json) for configuraiton.

If you do not have access to a RHMAP instance, you can sign up for a free instance at [https://openshift.feedhenry.com/](https://openshift.feedhenry.com/).

## How do I run it?  

### RHMAP Studio

This application and its cloud services are available as a project template in RHMAP as part of the "SAML Example Project" template.

### Local Clone (ideal for Open Source Development)
If you wish to contribute to this template, the following information may be helpful; otherwise, RHMAP and its build facilities are the preferred solution.

###  Prerequisites  
 * fh-js-sdk : 3.0.+
 * cordova: 4.0+

## Build instructions
 * npm install
 * Edit [fhconfig.json](www/fhconfig.json) to include the relevant information from RHMAP.  
 * cordova serve  

The `fh-js-sdk` and other development dependencies are defined in [package.json](package.json) and included in a [browserified script](www/js/main.js).
The [init.js](www/js/init.js) file is browserified and acts as a bridge between template script and npm dependencies. 
All the other JavaScript files in the template app will not be browserified, in order for you to be able to experiment live edit in RHMAP Studio preview.

## How does it work?

Click the "Sign In" button to sign in via your configured SAML IdP, this will open a webbrowser that you can use to login

