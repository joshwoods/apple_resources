

- UIKit
-  UIEventAttribution 

Class

# UIEventAttribution

An object that contains event attribution information for Web AdAttributionKit.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
class UIEventAttribution
```

## Overview

Apps use event attribution objects to send data to the browser when opening an external website that supports Web AdAttributionKit (formerly known as Private Click Measurement, or PCM). For more information on the proposed PCM web standard, see Introducing Private Click Measurement and Private Click Measurement Draft Community Group Report.

Note

Mac apps built with Mac Catalyst don’t support Web AdAttributionKit.

You can’t subclass UIEventAttribution.

### Define an endpoint

In order to use Web AdAttributionKit, your app defines an `Info.plist` key called NSAdvertisingAttributionReportEndpoint that contains the URL to which the browser sends event attribution data. When an externally linked website reports that a conversion has occurred, the browser forwards your app’s event attribution data to the endpoint specified in the `Info.plist`. If your app’s `Info.plist` doesn’t contain this key, the browser won’t be able to forward the Web AdAttributionKit data when a conversion occurs.

Send event attribution data to the browser only when your app opens an external link as a result of a user tapping a control that sits below a UIEventAttributionView in the app’s view hierarchy. The event attribution view verifies that the user tapped a control. If that control doesn’t sit below an event attribution view, the system won’t send the Web AdAttributionKit data to the browser when opening the external link.

### Create an event attribution data object

Here’s how you create a UIEventAttribution object:

- Swift
- Objective-C

```
let adURL = URL(string: "https://shop.example/tabletStandDeluxe.html")!
let eventAttribution =
    UIEventAttribution(sourceIdentifier: 4,
                       destinationURL: adURL,
                       sourceDescription: "Banner ad for Tablet Stand Deluxe.",
                       purchaser: "Shop Example, Inc.")
```

```
NSURL *adURL = [NSURL URLWithString:@"https://shop.example/tabletStandDeluxe.html"];
UIEventAttribution *eventAttribution = [[UIEventAttribution alloc]
                                        initWithSourceIdentifier:4
                                        destinationURL:adURL
                                        sourceDescription:@"Banner ad for Tablet Stand Deluxe."
                                        purchaser:@"Shop Example, Inc."];
```

### Send event attribution data to the browser

Once you create a UIEventAttribution object, send it to the browser when your app opens a URL as the result of a user tap. If the external website reports a conversion within 7 days, the browser forwards the data from the UIEventAttribution object to the specified remote server sometime between 24 and 48 hours after the conversion.

There are two different ways to send event attribution data when your app opens an external link, depending on whether your app uses UIScene or UIApplication for life cycle management. For more information on application life cycle management, see Managing your app’s life cycle.

Important

The browser, and not your app, sends the event attribution data to the remote server. If the user’s selected browser doesn’t support Web AdAttributionKit, the event attribution fails even if the external website reports a conversion.

If your app uses UIScene-based life cycle management, create a UIScene.OpenExternalURLOptions object, assign the event attribution object you created to its eventAttribution property, and call open(_:options:completionHandler:):

- Swift
- Objective-C

```
let sceneOpenURLOptions = UIScene.OpenExternalURLOptions()
sceneOpenURLOptions.eventAttribution = eventAttribution

self.view.window?.windowScene?.open(adURL,
                                    options: sceneOpenURLOptions,
                                    completionHandler: nil)
```

```
UISceneOpenExternalURLOptions *sceneOpenURLOptions = [[UISceneOpenExternalURLOptions alloc] init];
sceneOpenURLOptions.eventAttribution = eventAttribution;
[self.view.window.windowScene openURL:adURL
                                options:sceneOpenURLOptions
                    completionHandler:^(BOOL success) {
    if (success == NO) {
        // Handle error
    }
}];
```

If your app uses UIApplication-based life cycle management, create a dictionary that contains the eventAttribution key with the UIEventAttribution object you created as its value, and call open(_:options:completionHandler:), passing the dictionary using the `options` parameter.

- Swift
- Objective-C

```
let appOpenURLOptions: [UIApplication.OpenExternalURLOptionsKey : Any] = [
    .eventAttribution: eventAttribution
]
UIApplication.shared.open(adURL,
                          options: appOpenURLOptions,
                          completionHandler: nil)
```

```
NSDictionary *appOpenURLOptions = [NSDictionary dictionaryWithObject:eventAttribution forKey:UIApplicationOpenURLOptionsEventAttributionKey];

[[UIApplication sharedApplication] openURL:adURL
                                   options:appOpenURLOptions
                         completionHandler:^(BOOL success) {
    if (success == NO) {
        // Handle error
    }
}];
```

### Send event attribution data to SFSafariViewController

If your app displays a web page in SFSafariViewController after a person taps an ad, add a UIEventAttributionView subview to the ad view or control in order to measure taps. When a person taps the ad, follow these steps:

1.  Create an SFSafariViewController.Configuration object.

2.  Assign the UIEventAttribution object you created to the eventAttribution property of the SFSafariViewController.Configuration object.

3.  Initialize an SFSafariViewController instance with the configuration object, and present it. SFSafariViewController validates that a tap on a UIEventAttributionView initiated the navigation to the webpage. If not, it discards the attribution data.

## Topics

### Creating event attribution objects

init(sourceIdentifier: UInt8, destinationURL: URL, sourceDescription: String, purchaser: String)

Initializes a new event attribution object.

### Setting attribution details

var destinationURL: URL

The destination URL to attribute.

var purchaser: String

The entity that purchased the ad or content.

var reportEndpoint: URL?

The URL that receives attribution data.

var sourceDescription: String

A string describing the source tapped to launch the external link.

var sourceIdentifier: UInt8

A number that identifies the source of the attribution.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Private Click Measurement (PCM)

class UIEventAttributionView

An overlay view that verifies user interaction for Web AdAttributionKit.

NSAdvertisingAttributionReportEndpoint

The URL where Private Click Measurement and SKAdNetwork send attribution information.

