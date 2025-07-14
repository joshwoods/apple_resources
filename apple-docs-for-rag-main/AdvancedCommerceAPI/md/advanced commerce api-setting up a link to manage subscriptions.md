

- Advanced Commerce API
-  Setting up a link to manage subscriptions 

Article

# Setting up a link to manage subscriptions

Create a deep link to a subscription-management page for your app.

## Overview

Customers use the Settings \> Apple Account \> Subscriptions page in iOS to manage their subscriptions, including upgrading, downgrading, resubscribing, and canceling. When you offer subscriptions through the Advanced Commerce API, the Subscriptions page displays a “Manage in App” button.

You implement a subscription-management page in your app, and create a deep link URL to it that you submit to Apple. The Settings \> Apple Account \> Subscriptions page then uses your deep link for the “Manage in App” button.

Important

To submit the subscription-management deep link URL for your eligible Advanced Commerce API app, use the Advanced Commerce API Access form on the Advanced Commerce API page.

Create the deep link by following these guidelines:

- Follow universal link guidelines for the URL. For more information, see Allowing apps and websites to link to your content.

- Ensure the deep link lands on a page in your app that provides information about the subscription’s state and options for the customer to manage their subscription, for example, to change the plan, or resubscribe.

- Optionally, provide a unique subscription-management deep link URL for each storefront.

## See Also

### Essentials

Setting up your project for Advanced Commerce API

Configure your app in App Store Connect, set up your server, and prepare your SKUs.

Creating SKUs for your In-App Purchases

Define and manage one-time charges, subscriptions, and bundled subscriptions within your app.

Advanced Commerce API changelog

Learn about new features and updates in the Advanced Commerce API.

