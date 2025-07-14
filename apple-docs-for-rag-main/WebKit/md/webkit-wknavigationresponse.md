

- WebKit
-  WKNavigationResponse 

Class

# WKNavigationResponse

An object that contains the response to a navigation request, and which you use to make navigation-related policy decisions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKNavigationResponse
```

## Overview

Use a WKNavigationResponse object to make policy decisions about whether to allow navigation within your app’s web view. You don’t create WKNavigationResponse objects directly. Instead, the web view creates them and delivers them to the appropriate delegate objects. Use the methods of your delegate to analyze the response and determine whether to allow the resulting navigation to occur.

## Topics

### Getting the Response Details

var response: URLResponse

The frame’s response.

### Getting Additional Response Information

var canShowMIMEType: Bool

A Boolean value that indicates whether WebKit is capable of displaying the response’s MIME type natively.

var isForMainFrame: Bool

A Boolean value that indicates whether the response targets the web view’s main frame.

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

class WKNavigationAction

An object that contains information about an action that causes navigation to occur.

