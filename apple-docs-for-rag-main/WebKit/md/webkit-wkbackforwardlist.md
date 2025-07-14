

- WebKit
-  WKBackForwardList 

Class

# WKBackForwardList

An object that manages the list of previously loaded webpages, which the web view uses for forward and backward navigation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKBackForwardList
```

## Overview

Use a WKBackForwardList object to retrieve a web view’s previously loaded pages. Typically, you don’t create WKBackForwardList objects directly. Each web view creates one automatically and uses it to store the history of all loaded pages. Fetch this object from your web view’s backForwardList property and use its contents to facilitate programmatic navigation.

## Topics

### Getting the Most Recent Items

var backItem: WKBackForwardListItem?

The item immediately preceding the current item, if any.

var currentItem: WKBackForwardListItem?

The current item.

var forwardItem: WKBackForwardListItem?

The item immediately following the current item, if any.

### Getting Specific Items in the List

func item(at: Int) -> WKBackForwardListItem?

Returns the item at the relative offset from the current item.

### Getting Sublists

var backList: [WKBackForwardListItem]

The array of items that precede the current item.

var forwardList: [WKBackForwardListItem]

The array of items that follow the current item.

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

class WKBackForwardListItem

A representation of a webpage that the web view previously visited.

class WKNavigation

An object that tracks the loading progress of a webpage.

class WKNavigationAction

An object that contains information about an action that causes navigation to occur.

class WKNavigationResponse

An object that contains the response to a navigation request, and which you use to make navigation-related policy decisions.

