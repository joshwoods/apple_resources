

- WebKit
-  WKFindResult 

Class

# WKFindResult

An object that contains the results of searching the web view’s contents.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@MainActor
class WKFindResult
```

## Overview

When you perform a search using the methods of WKWebView, the web view creates a WKFindResult object and delivers it to your completion handler. You don’t create instances of this class directly. Use the objects that the web view provides to determine whether it found a match for the content.

## Topics

### Getting the Search Result

var matchFound: Bool

A Boolean value that indicates whether the web view found a match during the search.

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

### Page-Level Search

class WKFindConfiguration

The configuration parameters to use when searching the contents of the web view.

