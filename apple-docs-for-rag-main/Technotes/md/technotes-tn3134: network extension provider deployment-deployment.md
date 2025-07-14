

- Technotes
-  TN3134: Network Extension provider deployment 

Article

# TN3134: Network Extension provider deployment

Explore the platforms, packaging, OS versions, and device configurations for Network Extension provider deployment.

## Overview

Network Extension providers extend the networking stack in various ways. You might implement a custom VPN protocol with a packet tunnel provider, or add a content filter provider as part of a parental control app. Network Extension supports many different provider types and each type has different deployment requirements. The tables below summarise these requirements for each provider type.

When reading these tables:

- The Mac Catalyst platform refers to a provider embedded in a Mac Catalyst app running on Mac. For more information, see Mac Catalyst.

- The iOS Apps on Mac platform refers to a provider embedded in an iOS app running on an Apple silicon Mac. For more information, see Running your iOS apps in macOS.

- On macOS most Network Extension provider types can be packaged as either an app extension or a system extension. App extensions run in a user context; if the user logs out, the provider is terminated. System extensions run in a global context, completely independent of the logged in user.

- If a macOS row does not mention the “App Store only” restriction, the provider supports both App Store distribution and independent distribution using Developer ID signing.

For more information about using the Network Extension framework as a whole, see Network Extension.

## Deploying a packet tunnel provider

When building a packet tunnel provider, use the following table to plan your deployment:

| Platform | Packaged as | Minimum OS | Restrictions |
|----|----|----|----|
| iOS | app extension | 9.0 | per-app mode requires managed device |
| tvOS | app extension | 17.0 | per-app mode not supported |
| macOS | app extension | 10.11 | App Store only |
|  | system extension | 10.15 |  |
| Mac Catalyst | app extension | 10.15 | App Store only |
| iOS Apps on Mac | app extension | 11.0 | App Store only |

For more information, see Packet Tunnel Provider.

Before you decide to implement a packet tunnel provider, read TN3120: Expected use cases for Network Extension packet tunnel providers.

## Deploying an app proxy provider

When building an app proxy provider, use the following table to plan your deployment:

| Platform        | Packaged as      | Minimum OS | Restrictions         |
|-----------------|------------------|------------|----------------------|
| iOS             | app extension    | 9.0        | managed devices only |
| macOS           | app extension    | 10.11      | App Store only       |
|                 | system extension | 10.15      |                      |
| Mac Catalyst    | app extension    | 10.15      | App Store only       |
| iOS Apps on Mac | app extension    | 11.0       | App Store only       |

For more information, see App Proxy Provider.

## Deploying a content filter provider

When building a content filter provider, use the following table to plan your deployment:

| Platform | Packaged as      | Minimum OS | Restrictions                |
|----------|------------------|------------|-----------------------------|
| iOS      | app extension    | 9.0        | supervised devices only     |
|          | app extension    | 15.0       | apps using Screen Time APIs |
|          | app extension    | 16.0       | per-app on managed devices  |
| macOS    | system extension | 10.15      |                             |

For more information, see Content Filter Providers.

In the Screen Time case, content filters are only supported on child devices. To enable a content filter:

1.  Add the Family Controls capability to your app. See Adding capabilities to your app.

2.  Run it on a device where the user has signed in as an under 18 child member of an iCloud family.

3.  Request child authorization. On iOS 16 and later, call requestAuthorization(for:), passing in the `.child` option. On iOS 15, call requestAuthorization(completionHandler:), which always requests child authorization.

4.  Authorize that as the child’s parent or guardian.

Before submitting your app to the App Store, you must request permission to use the Family Controls entitlement for distribution.

## Deploying a DNS proxy provider

When building a DNS proxy provider, use the following table to plan your deployment:

| Platform | Packaged as      | Minimum OS | Restrictions               |
|----------|------------------|------------|----------------------------|
| iOS      | app extension    | 11.0       | supervised devices only    |
|          | app extension    | 16.0       | per-app on managed devices |
| macOS    | system extension | 10.15      |                            |

For more information, see DNS Proxy Provider.

## Deploying a transparent proxy provider

When building a transparent proxy provider, use the following table to plan your deployment:

| Platform | Packaged as      | Minimum OS | Restrictions   |
|----------|------------------|------------|----------------|
| macOS    | app extension    | 10.15      | App Store only |
|          | system extension | 10.15      |                |

For more information, see Network Extension.

macOS 11.0 introduced significant improvements to the transparent proxy feature; for the details, see the doc comments in ``.

## Deploying a packet filter provider

When building a packet filter provider, use the following table to plan your deployment:

| Platform | Packaged as      | Minimum OS |
|----------|------------------|------------|
| macOS    | system extension | 10.15      |

For more information, see Content Filter Providers.

## Deploying an Ethernet tunnel provider

When building an Ethernet tunnel provider, use the following table to plan your deployment:

| Platform | Packaged as      | Minimum OS | Restrictions   |
|----------|------------------|------------|----------------|
| macOS    | app extension    | 13.0       | App Store only |
|          | system extension | 13.0       |                |

For more information, see Network Extension.

## Deploying an app push provider

When building an app push provider, use the following table to plan your deployment:

| Platform | Packaged as   | Minimum OS |
|----------|---------------|------------|
| iOS      | app extension | 14.0       |

For more information, see Local Push Connectivity.

## Revision History

- **2023-11-28** Clarified the Family Controls behaviour for content filter providers on iOS.

- **2023-10-03** Updated for tvOS 17.

- **2022-09-06** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

