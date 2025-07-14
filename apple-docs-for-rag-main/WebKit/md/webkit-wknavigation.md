

- WebKit
-  WKNavigation 

Class

# WKNavigation

An object that tracks the loading progress of a webpage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKNavigation
```

## Overview

A WKNavigation object uniquely identifies a load request for a webpage. When you ask a web view to load content or navigate to a page, the web view returns a WKNavigation object that identifies your request. As the load operation progresses, the web view reports progress of that operation to various methods of its navigation delegate, passing them the matching WKNavigation object.

## Topics

### Getting the Content Mode

var effectiveContentMode: WKWebpagePreferences.ContentMode

The content mode WebKit uses to load the webpage.

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

class WKNavigationAction

An object that contains information about an action that causes navigation to occur.

class WKNavigationResponse

An object that contains the response to a navigation request, and which you use to make navigation-related policy decisions.

