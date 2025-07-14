

- Screen Time
-  STWebpageController 

Class

# STWebpageController

The controller you use to report web usage and block restricted webpages.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor
class STWebpageController
```

## Overview

This class provides a convenient way for you to communicate changes in each webpage, such as when the user starts or stops playing media. When a parent or guardian of the user blocks the webpage’s current URL, the webpage controller:

- Automatically occludes the web page’s content

- Updates a KVO-compliant urlIsBlocked property

For example, you can observe `urlIsBlocked` and take action when it changes to YES, such as pausing media.

Important

Create a webpage controller for each webpage or tab and add it on top of the webpage’s content.

## Topics

### Instance properties

var suppressUsageRecording: Bool

A Boolean that indicates whether the webpage controller is not recording web usage.

var url: URL?

The URL for the webpage.

var urlIsBlocked: Bool

A Boolean that indicates whether a parent or guardian has blocked the URL.

var urlIsPictureInPicture: Bool

A Boolean that indicates whether the webpage is currently displaying a floating picture in picture window.

var urlIsPlayingVideo: Bool

A Boolean that indicates whether there are one or more videos currently playing in the webpage.

### Instance methods

func setBundleIdentifier(String) throws

Changes the bundle identifier used to report web usage.

### Instance Properties

var profileIdentifier: STWebHistory.ProfileIdentifier?

An optional identifier for the current browsing profile.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

