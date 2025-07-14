

- Technotes
-  TN3165: Packet Filter is not API 

Article

# TN3165: Packet Filter is not API

Plan your migration from Packet Filter to Network Extension.

## Overview

macOS implements the BSD Packet Filter mechanism. This has two expected use cases:

- As an implementation detail of various system services built-in to macOS

- As an advanced feature for users, site admins, and so on

It is not considered API. Do not use Packet Filter in a software product that you distribute to a wide audience. If you’re currently shipping software that relies on Packet Filter, plan to migrate to Network Extension.

## Packet Filter fundamentals

Packet Filter, oftened shorted to just PF or even pf, shows up in a number of places:

- The `/dev/pf` character device

- Various `/etc/pf*` configuration files

- The `pfctl` command-line tool

- The `pfctl` and `pf.conf` man pages

PF implements rule-based filtering. These rules are manipulated by various system services and, less commonly, by the user. PF is not considered API because the PF rules you install might clash with those installed by:

- The user

- macOS system services, either now or in the future

- Other third-party products

## Moving off packet filter

If you’re currently shipping a product based on PF, plan to migrate it to a supported API. In most cases that means creating a Network Extension provider:

- If your product is a VPN, create either a packet tunnel or app proxy provider.

- If your product looks at, and potentially blocks, TCP connections or UDP flows, create a content filter provider.

- If your product looks at, and potentially blocks, network packets, create a packet filter provider.

- If your product wants to intercept DNS queries, create a DNS proxy provider.

- If none of these providers meet your specific needs, create a transparent proxy provider.

For information about packaging and OS version constraints, see TN3134: Network Extension provider deployment.

If your product needs to do something that’s not covered by one of these providers, use Feedback Assistant to let us know what’s missing.

## Test during the transition

It may take you some time to migrate from PF to Network Extension. In the meantime, test your existing product to ensure that it’s compatible with various macOS system services. Specifically, test with:

- Mac Virtual Display for visionOS devices

- Xcode

- Internet Sharing

- AirDrop

- Other Continuity features

Also, consider testing with products from other third-party developers who work in this space.

When testing with Xcode, check that you can build, run, and debug an app on your iOS device over the network. Then repeat this test with the device connected via USB. Xcode 15 and later use the networking stack to communicate with the iOS device even when it’s directly connected.

If you set up these tests with your existing product, you’ll be able to reuse them to validate the functionality of your Network Extension based product.

## Revision History

- **2024-02-27** First published.

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

