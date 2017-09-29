Magento: Two-Factor-Authentication
=====================
[![Build Status](https://travis-ci.org/magento-hackathon/Magento-Two-factor-Authentication.svg?branch=master)](https://travis-ci.org/magento-hackathon/Magento-Two-factor-Authentication) [![Code Climate](https://codeclimate.com/github/magento-hackathon/Magento-Two-factor-Authentication/badges/gpa.svg)](https://codeclimate.com/github/magento-hackathon/Magento-Two-factor-Authentication)

Implementation of an two-factor-authentication using Google's 2-Step Verification algorithm.

### Abstract

Admin (backend) users whose role's resources are in the list of protected resources,
are asked to enter one-time security code generated by the Google Authenticator app on their mobile phone after
they have authenticated themselves in the admin by using standard login dialog.
This ensures that critical resources in the admin have extra protection layer that cannot be accessed
by third parties without one-time security code. It includes cases when someone's laptop is stolen or accessed
by third parties.

> **NOTE:**
> Default login will be also required to login!
> 2FA is only an additional login to increase the security.

### How to use it

- Install [Google Authenticator](https://support.google.com/accounts/answer/1066447?hl=de) app to your smartphone
- Install this extension via [Composer](https://getcomposer.org/) or [modman](https://github.com/colinmollenhour/modman)
- Log in to Magento admin
- You will be requested to scan the QR code with the Google Authenticator app and define security questions
- Continue Log in

### Installation using Composer

Add `"magento-hackathon/magento-two-factor-authentication": "*"` to the `require` section of your `composer.json` file or
add it by calling the Composer shell command:

    composer require magento-hackathon/magento-two-factor-authentication:*

### Contributors

This project was initiated at the Magento Worldwide Online Hackathon, Januar 2014 and started as a proof-of-concept. The project was continued during the Pre-Imagine MageHackathon on May 11, 2014 and received further updates and maintenance from community members after this time.

### License

MIT License (MIT)


[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fclivewalkden%2FMagento-Two-factor-Authentication.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fclivewalkden%2FMagento-Two-factor-Authentication?ref=badge_large)

### Fancy Images

#### Admin-Usage

##### Step 1 - Login in Admin-Panel

![Login in Admin](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Admin-Step1-Login.png?raw=true)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fclivewalkden%2FMagento-Two-factor-Authentication.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fclivewalkden%2FMagento-Two-factor-Authentication?ref=badge_shield)

##### Step 2 - Link Admin with Google Authenticator - just scan the Barcode

![Link account to AuthenticatorApp](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Admin-Step2-Link.png?raw=true)

##### Step 3 - Redirect to "Two-Factor Authentication Setup"

![My Account in Admin](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Admin-Step3-MyUser.png?raw=true)

##### After inital setup everything is simpler:

###### Login

![Login in Admin](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Admin-Step1-Login.png?raw=true)

###### Enter code after Login

![Enter code from Authenticator](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Admin-Step4-EnterCodeAfterLogin.png?raw=true)

#### Customer-Usage

##### Step 1 - Customer-Login

![Login in customer account](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Customer-Step1-Login.png?raw=true)

##### Step 2 - Find the menu in customer account

![Click the link](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Customer-Step2-FindIt.png?raw=true)

##### Step 3 - activate it for customer

![Activate Two-Factor-Authentication for customer account](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Customer-Step3-Link.png?raw=true)

##### After inital setup everything is simpler:

###### Login

![Customer login](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Customer-Step1-Login.png?raw=true)

###### Enter code after Login

![Enter code from Authenticator](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Customer-Step4-EnterCodeAfterLogin.png?raw=true)

#### Recovery

##### Reset token for admin-user (other account with access needed of course)

![Reset token for user](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Admin-EditUser.png?raw=true)

##### Reset Token for customer (admin-access needed)

![Reset token for customer](https://github.com/magento-hackathon/Magento-Two-factor-Authentication/blob/readme-images/readme-images/Admin-EditCustomer.png?raw=true)