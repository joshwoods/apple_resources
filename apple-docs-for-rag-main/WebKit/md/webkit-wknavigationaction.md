

- WebKit
-  WKNavigationAction 

Class

# WKNavigationAction

An object that contains information about an action that causes navigation to occur.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKNavigationAction
```

## Overview

Use a WKNavigationAction object to make policy decisions about whether to allow navigation within your app’s web view. You don’t create WKNavigationAction objects directly. Instead, the web view creates them and delivers them to the appropriate delegate objects. Use the methods of your delegate to analyze the action and determine whether to allow the resulting navigation to occur.

## Topics

### Getting the navigation type

var navigationType: WKNavigationType

The type of action that triggered the navigation.

enum WKNavigationType

The type of action that triggered the navigation.

### Inspecting navigation information

var request: URLRequest

The URL request object associated with the navigation action.

var sourceFrame: WKFrameInfo

The frame that requested the navigation.

var targetFrame: WKFrameInfo?

The frame in which to display the new content.

var shouldPerformDownload: Bool

A Boolean value that indicates whether the web content provided an attribute that indicates a download.

### Inspecting user actions

var buttonNumber: UIEvent.ButtonMask

The number of the mouse button that caused the navigation request.

var modifierFlags: UIKeyModifierFlags

The modifier keys that were pressed at the time of the navigation request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Navigation

protocol WKNavigationDelegate

Methods for accepting or rejecting navigation changes, and for tracking the progress of navigation requests.

class WKBackForwardList

An object that manages the list of previously loaded webpages, which the web view uses for forward and backward navigation.

class WKBackForwardListItem

A representation of a webpage that the web view previously visited.

class WKNavigation

An object that tracks the loading progress of a webpage.

class WKNavigationResponse

An object that contains the response to a navigation request, and which you use to make navigation-related policy decisions.

