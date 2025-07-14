

- WebKit
-  WKFrameInfo 

Class

# WKFrameInfo

An object that contains information about a frame on a webpage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKFrameInfo
```

## Overview

An instance of this class is a transient, data-only object; it does not uniquely identify a frame across multiple delegate method calls.

## Topics

### Inspecting frame information

var isMainFrame: Bool

A Boolean value indicating whether the frame is the web site’s main frame or a subframe.

var request: URLRequest

The frame’s current request.

var securityOrigin: WKSecurityOrigin

The frame’s security origin.

var webView: WKWebView?

The web view that contains this frame and the containing webpage.

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

### Page Content

class WKUserContentController

An object for managing interactions between JavaScript code and your web view, and for filtering content in your web view.

class WKContentRuleListStore

An object that contains the rules for how to load and filter content in the web view.

class WKContentWorld

An object that defines a scope of execution for JavaScript code, and which you use to prevent conflicts between different scripts.

class WKSecurityOrigin

An object that identifies the origin of a particular resource.

class WKUserScript

A script that the web view injects into a webpage.

