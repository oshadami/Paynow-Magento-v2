Sage Pay Now Credit Card Payment Module for Magento v2+
=======================================================

Revision 1.0.0

Introduction
------------
A credit card module to take credit card transaction for Magento using Sage Pay South Africa's Pay Now gateway.

Installation Instructions
-------------------------
Download the files from GitHub:

> https://github.com/SagePay/PayNow-Magento-2/archive/master.zip

1. Setup **ZAR** on your Magento site. In the admin panel navigate to 'Stores', and add ZAR under currency Symbols and Rates.
2. Copy the Paynow app folder to your root Magento folder.
    This will not override any files on your system.
3. You will now need to run the following commands in the given order:
    - php ./bin/magento module:enable Paynow_Paynow
    - php ./bin/magento setup:di:compile
    - php ./bin/magento setup:static-content:deploy
    - php ./bin/magento cache:clean
4. Log into the admin panel and navigate to Stores > Configuration > Sales > Payment Method and click on Paynow
5. Enable the module, as well as debugging.
6. Add your Pay Now Service Key
7. Click 'Save Config'

Configuration
-------------

#### Prerequisites:

You will need:

* Sage Pay Now login credentials
* Sage Pay Now Service key
* Magento admin login credentials

#### Sage Pay Now Gateway Server Configuration Steps:

1. Log into your Sage Pay Now Gateway Server configuration page (https://merchant.sagepay.co.za/SiteLogin.aspx)
2. Go to Account / Profile
3. Click Sage Connect
4. Click Pay Now
5. Make a note of your Service key

#### Sage Pay Now Callback

6. Choose the following for your Accept, Decline, Notify & Redirect URLs:

> http://domain.co.za/paynow/notify/

Issues & Feature Requests
-------------------------

We welcome your feedback.

Please contact Sage Pay South Africa with any questions or issues.
