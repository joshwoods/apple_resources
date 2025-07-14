

- WebKit
-  WKBackForwardListItem 

Class

# WKBackForwardListItem

A representation of a webpage that the web view previously visited.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKBackForwardListItem
```

## Overview

Use a WKBackForwardListItem object to get information about previously visited webpages. This object identifies the page’s title and URL. It also identifes the URL that requested the webpage.

You don’t create WKBackForwardListItem objects directly. Instead, a WKBackForwardList object creates them in conjunction with its associated web view when the web view loads new pages.

## Topics

### Getting the Page-Specific Information

var title: String?

The title of the webpage this item represents.

var url: URL

The URL of the webpage this item represents.

### Getting the Requesting Page

var initialURL: URL

The source URL that originally asked the web view to load this page.

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

class WKNavigation

An object that tracks the loading progress of a webpage.

class WKNavigationAction

An object that contains information about an action that causes navigation to occur.

class WKNavigationResponse

An object that contains the response to a navigation request, and which you use to make navigation-related policy decisions.

