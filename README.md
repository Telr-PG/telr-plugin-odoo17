# Telr Payments Plugin for Odoo #

This plugin enables your Odoo powered platform to start accepting payments via Telr.

### Process to Enable Telr Payment Gateway ###

1)	Activate developer mode
	  * Log in Odoo Admin Portal, navigate to Settings > General Settings > Activate the developer mode to activate.	
2)  Install custom add-on
      * The contents of the zip file should be copied into /customaddons folder which will be found in the root directory of your Odoo installation. 
      * If customaddons directory is not available in the root directory, then create the “customaddons” directory and mention the customaddons path in “debain/odoo.conf” file under the addons_path variable and restart the odoo server      
3)	Activate custom add-on
* Add your 'Store ID' and 'Authentication Key' in the admin panel (Note : If you have not 'Store ID' and 'Authentication Key' please contact with Telr support)

Note: The payment provider depends on other add-ons like "Generic - Accounting", "Sale", "eCommerce", “Website”, please install these required dependencies in advance.

### Configuring Odoo ###

* In Odoo admin system, Navigate Website > Configuration > eCommerce > Payment providers and click on the “Telr Payment” option.
* In Odoo admin system, Navigate Website > Configuration > eCommerce > Payment method > Card > Configuration and search “Telr Payment” option in “Supported by” and selected.
* Then you need to edit the settings for the payment method. For test mode select the “Test Mode” state and for live mode select the “Enable” option. 
* In credential tab enter your Telr Store ID, Authentication Key.
* Your Telr Store ID is displayed in the top right of the Telr Merchant Administration System, and you must only copy the numeric part of the ID, not the full store name. You will get the authentication key in Telr Merchant Administration System in Hosted Payment Page V2 configuration page, under the Integrations menu.
* In Configuration Tab, you can set the payment mode, payment language and payment transaction mode. Therse are the optional fields.

### IP Whitelisting for Live Transactions ###

	Before processing live transactions, ensure that the IP of your server system are updated into the Payment Page V2 configuration in the Telr Merchant Administration System.

## License

This repository is available under the [MIT license](LICENSE).
