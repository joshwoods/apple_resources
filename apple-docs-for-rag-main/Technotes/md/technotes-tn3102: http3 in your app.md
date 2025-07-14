

- Technotes
-  TN3102: HTTP/3 in your app 

Article

# TN3102: HTTP/3 in your app

Get started with iOS 15’s new HTTP/3 support.

## Overview

HTTP/3 is a major new feature in iOS 15. While you wait for your server to add support for it, here’s how you can test it today in your app:

1.  Make sure your test device is running iOS 15 or later (`HTTP/3` is not supported in the simulator).

2.  In Settings \> Developer, under the Networking group, enable `HTTP/3`.

3.  Using Xcode 13.0 or later, create a new project from the iOS \> App template. Set the Language popup to Swift and the Interface popup to SwiftUI.

4.  Change the `HTTP3App.swift` and the `ContentView.swift` files to the code shown below.

5.  Run the app on your device.

6.  Tap your Test button.

```
```

## Testing notes

After running the code above, your app will print something similar to:

```
task will start, url: 
protocols: ["h3-29"] // ["h3", "h2"]
task finished with status 200, bytes 703
```

The protocols array shows the protocol used for each HTTP transaction. In this case there was a single `HTTP/3` transaction. In some cases you may see the protocol being returned as `h2` or even `http1.1`. If this is the case then run the transaction again. This gives URLSession the opportunity to apply the `HTTP/3` service discovery option that your server sent back on the previous HTTP response.

Service discovery for `HTTP/3` is performed in one of the following ways:

- The recommended approach is to configure your DNS server to advertise the HTTPS resource record for `alpn="h3,h2"`.

- Alternatively, configure your server to respond back with the `Alt-Svc` header that advertises `HTTP/3`. For example, `Alt-Srv: h3=":443"; ma=2592000`.

To attempt to use `HTTP/3` on the first transaction, set the assumesHTTP3Capable property on the URLRequest being used to execute the data task in URLSession.

For cases where `HTTP/3` is not supported on the server, or over the network, you will see the protocol fall back to `h2` or `http1.1`. For more information on this, please see the WWDC session for Accelerate networking with HTTP/3 and QUIC.

Note

Servers that support `HTTP/3` need to be based on Draft 29 or later.

If you experience issues while debugging your network transactions, take a look at these requests in the Network Instruments tool to debug what you are seeing being sent back from your server. For more on this, see the article for Analyzing HTTP Traffic with Instruments.

## Revision History

- **2022-05-24** Made minor editorial changes.

- **2022-02-08** Republished as TN3102.

- **2021-06-16** First published as “HTTP/3 in Your App” on the Apple Developer Forums.

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

