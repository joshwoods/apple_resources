

- UIKit
-  UIEventAttributionView 

Class

# UIEventAttributionView

An overlay view that verifies user interaction for Web AdAttributionKit.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
class UIEventAttributionView
```

## Overview

Web AdAttributionKit (formerly known as Private Click Measurement, or PCM) is a proposed web standard that allows external websites to measure when external links, such as ads, result in a *conversion*. The external website decides what constitutes a conversion, but it’s often the result of the user making a purchase or signing up for a service. Web AdAttributionKit doesn’t send any user-identifiable information to the remote server, so it protects user privacy, while providing websites the ability to measure the effectiveness of their ad campaigns.

Apps running in iOS 17.4 or later can use AdAttributionKit to record click-through impressions on custom rendered ad content using a `UIEventAttributionView`. For more information about click-through in AdAttributionKit, see Presenting ads in your app.

Apps running in iOS 14.5 or later can take advantage of Web AdAttributionKit by sending event attribution data to the browser when opening an external link. If the linked website reports a conversion within 7 days, the browser forwards your appʼs Web AdAttributionKit data to a specified remote server sometime between 24 and 48 hours after the reported conversion.

You can’t subclass UIEventAttributionView.

For more information on the proposed Web AdAttributionKit web standard, see Introducing Private Click Measurement and Private Click Measurement Draft Community Group Report.

### Verify user interaction

Event attribution views overlay other UIKit controls to ensure that either handling a tap with `AdAttributionKit` or opening an external link with Web AdAttributionKit data only happens as the result of a user tap. The system doesn’t handle the tap or send event attribution data to the browser unless a `UIEventAttributionView` exists above the tapped control.

### Create an event attribution view

Place an event attribution view above any view that launches external links with event attribution data and make sure there are no other overlapping views above the event attribution view that might intercept taps. UIEventAttributionView doesn’t consume tap events, so the behavior of any control below one in the view hierarchy isn’t affected.

If multiple views or controls in your app can launch an external link using Web AdAttributionKit, use a separate UIEventAttributionView to overlay each control. While you can use a single UIEventAttributionView to validate more than one control, attribution views that cover large portions of the screen may impact performance because the system must validate all user interactions that pass through the attribution view.

Here’s how to add an event attribution view to an in-app advertisement:

- Swift
- Objective-C

```
// Create an event attribution view.
let eventAttributionView = UIEventAttributionView()

// Place it over the ad view.
eventAttributionView.translatesAutoresizingMaskIntoConstraints = false
adView.addSubview(eventAttributionView)
NSLayoutConstraint.activate([
    adView.topAnchor.constraint(equalTo: eventAttributionView.topAnchor),
    adView.leadingAnchor.constraint(equalTo: eventAttributionView.leadingAnchor),
    adView.trailingAnchor.constraint(equalTo: eventAttributionView.trailingAnchor),
    adView.bottomAnchor.constraint(equalTo: eventAttributionView.bottomAnchor)
])
```

```
// Create an event attribution view.
UIEventAttributionView *eventAttributionView = [[UIEventAttributionView alloc] init];

// Place it over the ad view.
eventAttributionView.translatesAutoresizingMaskIntoConstraints = NO;
[adView addSubview:eventAttributionView];
[NSLayoutConstraint activateConstraints: @[
    [adView.topAnchor constraintEqualToAnchor:eventAttributionView.topAnchor],
    [adView.leadingAnchor constraintEqualToAnchor:eventAttributionView.leadingAnchor],
    [adView.trailingAnchor constraintEqualToAnchor:eventAttributionView.trailingAnchor],
    [adView.bottomAnchor constraintEqualToAnchor:eventAttributionView.bottomAnchor]
]];
```

For more information on sending Web AdAttributionKit event attribution data to the browser when opening an external link, see UIEventAttribution.

Note

Web AdAttributionKit isn’t supported in Mac apps built with Mac Catalyst.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Private Click Measurement (PCM)

class UIEventAttribution

An object that contains event attribution information for Web AdAttributionKit.

NSAdvertisingAttributionReportEndpoint

The URL where Private Click Measurement and SKAdNetwork send attribution information.

