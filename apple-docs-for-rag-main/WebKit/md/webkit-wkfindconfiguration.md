

- WebKit
-  WKFindConfiguration 

Class

# WKFindConfiguration

The configuration parameters to use when searching the contents of the web view.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@MainActor
class WKFindConfiguration
```

## Overview

Create a WKFindConfiguration object and configure its attributes to specify how to perform searches within the web view’s contents. To initiate a search, call the appropriate method of WKWebView and pass this object along with the search string.

## Topics

### Configuring the Search Parameters

var backwards: Bool

A Boolean value that indicates the search direction, relative to the current selection.

var caseSensitive: Bool

A Boolean value that indicates whether to consider case when matching the search string.

var wraps: Bool

A Boolean value that indicates whether the search wraps around to the other side of the page.

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

### Related Documentation

func find(String, configuration: WKFindConfiguration, completionHandler: (WKFindResult) -> Void)

Searches for the specified string in the web view’s content.

### Page-Level Search

class WKFindResult

An object that contains the results of searching the web view’s contents.

