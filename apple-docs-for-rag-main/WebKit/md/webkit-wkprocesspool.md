

- WebKit
-  WKProcessPool 

Class

# WKProcessPool

An opaque token that you use to run multiple web views in a single process.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKProcessPool
```

## Overview

A WKProcessPool object represents a single process that WebKit uses to manage web content. To provide a more secure and stable experience, WebKit renders the content of web views in separate processes, rather than in your app’s process space. By default, WebKit gives each web view its own process space until it reaches an implementation-defined process limit. After that, web views with the same WKProcessPool object share the same web content process.

If your app creates multiple web views, assign the same WKProcessPool object to web views that may safely share a process space. Instantiate an instance of this class and assign it to the processPool property of each web view’s WKWebViewConfiguration object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Web View Configuration

class WKWebViewConfiguration

A collection of properties that you use to initialize a web view.

class WKWindowFeatures

Display-related attributes that a webpage requests for its window.

class WKPreferences

An object that encapsulates the standard behaviors to apply to websites.

class WKWebpagePreferences

An object that specifies the behaviors to use when loading and rendering page content.

