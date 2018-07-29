=== Event Tracking for Gravity Forms ===
Contributors: ronalfy, bigwing, nmarks, kzeni
Tags: gravity forms, google analytics, google tag manager, matomo, piwik, event tracking
Requires at least:4.0
Tested up to: 4.9
Stable tag: 2.1.1
Requires PHP: 5.6
Donate link: https://mediaron.com/contribute/
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Easily add event tracking using Gravity Forms and your Google Analytics, Google Tag Manager, or Matomo (formerly Piwik) account.

== Description ==

This plugin provides an easy way to add event tracking to your Gravity Forms using Google Analytics, Google Tag Manager, or Matomo (formerly Piwik).

https://www.youtube.com/watch?v=rHW3roCuNSI&t=2s

Also supports:

* Pagination events
* JS only events
* Google Tag Manager
* Matomo (formerly Piwik)

= Setup Guide =
Looking for help setting things up? [Read Our Setup Guide](https://mediaron.com/event-tracking-for-gravity-forms/)

= Minimum Requirements =
- Gravity Forms 2.0+
- Google Analytics Universal Analytics
- Google Tag Manager (optional)
- Matomo (formerly Piwik) account (optional)

= Features =
- Submit events to Google Analytics using the Measurement Protocol, JavaScript, or using Google Tag Manager
- Submit events using Matomo (formerly Piwik)
- Add multiple event feeds with conditionals
- Custom event categories, actions, labels and even values
- Track form pagination events
- Dynamic event value on payment forms (integration with the payment add-ons including Paypal Standard, PayPal Pro, Stripe, etc...)

For payment based forms, you can leave the value blank to convert using the total payment amount.

<h3>Help Contribute</h3>

* Leave a star rating
* <a href="https://translate.wordpress.org/projects/wp-plugins/gravity-forms-facebook-pixel-tracking">Contribute a translation</a>
* <a href="https://github.com/ronalfy/wordpress-gravity-forms-event-tracking">Contribute some code</a>

== Installation ==

= Minimum Requirements =
- Gravity Forms 2.0+

= Using The WordPress Dashboard =

1. Navigate to the 'Add New' in the plugins dashboard
2. Search for gravity-forms-facebook-pixel-tracking
3. Click 'Install Now'
4. Activate the plugin on the Plugin dashboard

= Uploading in WordPress Dashboard =

1. Navigate to the 'Add New' in the plugins dashboard
2. Navigate to the 'Upload' area
3. Select `gravity-forms-event-tracking.zip` from your computer
4. Click 'Install Now'
5. Activate the plugin in the Plugin dashboard

= Using FTP =

1. Download `gravity-forms-event-tracking.zip`
2. Extract the `gravity-forms-event-tracking` directory to your computer
3. Upload the `gravity-forms-event-tracking` directory to the `/wp-content/plugins/` directory
4. Activate the plugin in the Plugin dashboard


== Frequently Asked Questions ==

= How do I track pagination? =

<a href="https://mediaron.com/event-tracking-for-gravity-forms/pagination/">Read our Guide on Pagination</a>.

= How do I track using JavaScript only? =

See <a href="https://mediaron.com/event-tracking-for-gravity-forms/google-analytics-mode/">Going Advanced</a>.

= Does this work with Google Tag Manager =

Yes. <a href="https://mediaron.com/event-tracking-for-gravity-forms/google-tag-manager/">Read our Guide on Google Tag Manager</a>.

= Are there any filters/hooks? =

Check out the documentation on [github](https://github.com/ronalfy/wordpress-gravity-forms-event-tracking)

== Screenshots ==

1. The Gravity Forms setting screen where you setup your event tracking.
2. The form settings feed list.
3. The feed settings page

== Changelog ==

= 2.1.1 = 
* Released 2018-06-22
* Documentation update

= 2.1.0 =
* Released 2018-01-10
* Enhancement: Added Matomo (formerly Piwik) support

= 2.0.9 =
* Released 2017-11-29
* Bug fix: added host name to measurement protocol due to filters blocking the conversion.
* Bug fix: fixed document location using the measurement protocol
* Bug fix: changed measurement protocol server-to-server call to something less strict to prevent inadvertent blocking on some servers.

= 2.0.7 =
* Released 2017-11-03
* Bug fix: events were not being sent using the measurement protocol on some installations

= 2.0.5 =
* Released 2017-10-17
* Bug fix: events were not being sent using the measurement protocol
* Bug fix: fixing various conflicts with PHP7.

= 2.0.3 =
* Released 2016-09-24
* Bug fix: Conflict with role management plugins

= 2.0.1 =
* Released 2016-09-23
* Bug fix: Google Tag Manager had an extra "s" in the action dataLayer variable.

= 2.0.0 =
* Released 2016-09-22
* Enhancement: Can track pagination events
* Enhancement: Can track events using JavaScript only (a highly requested feature)
* Enhancement: Can use Google Tag Manager

= 1.7.3 =
* Bugfix - Some users were experiencing PHP fatal errors upon form submission. Reverting to previously used library.

= 1.7.1 =
* Released 2016-03-28
* Hotfix - Removing SSL requirement. Needs more testing.

= 1.7.0 =
* Released 2016-03-28
* Plugin will now display an error if an incompatible version of PHP is installed.
* Bug Fix: Plugin no longer shows a notice if a UA code isn't set
* Bug Fix: Plugin will now trigger events if a UA code is set in the feed but not in the settings
* Enhancement: Document Path will now be set as part of event creation
* Enhancement: Measurement protocol updated
* Enhancement: Measurement protocol will not detect SSL and use the appropriate protocol

= 1.6.5 =
* Released 2015-12-11
* Ability to add multiple UA codes in the feed settings.

= 1.6.4 =
* Released 2015-09-22
* Testing with WordPress 4.3.
* Better internationalization

= 1.6.3 =
* Released 2015-02-10
* Integration with members plugin

= 1.6.2 =
* Released 2015-02-06
* Fixed bug where manual event values were not sent properly.

= 1.6.1 =
* Released 2015-01-28
* Hotfix to remove echo'd text bug

= 1.6.0 =
* Released 2015-01-25
* Refactored the plugin to use feeds. Now you can have multiple feeds with conditions!

= 1.5.5 =
* Released 2015-01-19
* Hotfix for issue with paypal standard converting early

= 1.5.3 =
* Released 2014-12-20
* Ensured page title and location are properly being sent to Google

= 1.5.2 =
* Released 2014-12-16
* Hotfix for PHP strict standards warning

= 1.5.0 =
* Released 2014-12-15
* Moved the form specific settings to their own tab.
* Re-structured the plugin code to fall in line with the official Gravity Forms plugins.
* Added a disable option to prevent a form from tracking any events.
* Added merge tag (choose a form field dropdown) to the settings fields for more dynamic tracking capabilities.

= 1.4.5 =
* Released 2014-12-04
* Fixed a bug where the source/medium was not being tracked correctly for PayPal Standard IPN Notification based conversions.

= 1.4.4 =
* Released 2014-12-03
* Added some information to the event settings section

= 1.4.3 =
* Released 2014-12-02
* Fixed backwards-compat issue

= 1.4 =
* Released 2014-12-01-
* Added value for events
* Properly integrated with payment based forms

= 1.3 =
* Properly integrated with Gravity Forms settings API (thanks ronalfy!)
* Enabled custom category/action/label on a per form basis.

== Upgrade Notice ==

= 2.1.0 =
Enhancement: Added Matomo (formerly Piwik) support