

- StoreKit
- In-App Purchase
- Original API for In-App Purchase
- Subscriptions and offers
-  Offering a Subscription Across Multiple Apps 

Article

# Offering a Subscription Across Multiple Apps

Support a single auto-renewable subscription across multiple apps.

## Overview

You can offer customers auto-renewable subscription services that are accessible through multiple apps across one or more operating systems.

To offer this functionality, your server must grant access to the subscription content across all apps, despite the user having purchased the subscription within a specific app. You can use a unified account management database along with server-side receipt validation to validate a user’s purchase and handle in-app transactions. By entitling subscription access from your server, you can provide users the ability to access your subscription across multiple apps.

### Create the Subscription for Each App

To get started, use App Store Connect to create a separate and equivalent auto-renewable subscription for each app that offers the multi-app subscription so that users can subscribe from any app. For design guidance, see Human Interface Guidelines > In-App Purchase.

Tip

Use an app bundle to group apps that share auto-renewable subscriptions on the same platform in a single App Store product page. An app bundle enables customers to view and download apps in a single purchase.

The following image illustrates the steps for implementing a multi-app subscription:

### Authenticate the User

When providing auto-renewable subscription access across multiple apps, you must authenticate the user in a way that correlates across apps. Authenticating users using a login allows you to determine if the user has access to the content. To provide a consistent user experience, ensure that the login process is similar across your apps.

To provide an easy and secure login, take advantage of Sign in with Apple. Sign in with Apple allows you to identify a user across your apps, while maintaining user privacy and protecting your app against fraud. You can store and retrieve user account data across your apps and the user’s devices, and use that data to unlock access appropriately.

### Check Billing Status

After authenticating the user, determine whether to grant access to the content based on their transaction history in the receipt.

Check if the user has purchased any subscription products before showing a subscription offer in the app. If there’s a subscription purchase from any app, verify if the subscription is active by looking at the subscription expiration date in the receipt.

Present users who don’t have an active subscription with the subscription for purchase. Consider all potential billing scenarios within your account database when determining eligibility and granting access to a user.

Important

If the user has purchased the subscription from an app, you must propagate the purchase across all the apps that provide the subscription service. Failing to persist the purchase to the other apps opens the possibility of a user paying multiple times for the same service.

### Validate Subscription Status

A user’s subscription status can change any time. Validate the receipt and check the latest subscription expiration date to maintain the billing status for each user and reflect any changes.

Enabling App Store Server Notifications keeps your server aware of changes made to a customer’s subscription status. Update your records to keep users’ subscription status and content current. The billing status must be accurate in your account database to provide the expected user experience across all apps.

### Enable Access to Purchased Content

After determining that the user should have access, you can enable access in each app based on the subscription expiration date. The user can access the subscription within any app that offers the same service. Repeat the previous steps as necessary across each app or user’s session to unlock the subscription.

## See Also

### Essentials

Handling Subscriptions Billing

Build logic around the date and time constraints of subscription products, while planning for all scenarios where you control access to content.

Enabling App Store Server Notifications

Configure your server and provide an HTTPS URL to receive notifications about in-app purchase events and unreported external purchase tokens.

Reducing Involuntary Subscriber Churn

Prevent unintentional loss of subscribers due to billing issues.

