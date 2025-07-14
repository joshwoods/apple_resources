

- WebKit
-  WKSecurityOrigin 

Class

# WKSecurityOrigin

An object that identifies the origin of a particular resource.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
class WKSecurityOrigin
```

## Overview

A WKSecurityOrigin object is a transient, data-only object that identifies the host name, protocol, and port number associated with a particular resource. You don’t create WKSecurityOrigin objects directly. Instead, WebKit creates them for the resources it loads. A *first-party* load is any load URL has the same security origin as the requesting web site. First-party webpages can access each other’s resources, such as scripts and databases.

Because a WKSecurityOrigin object is transient, it doesn’t uniquely identify a security origin across multiple delegate method calls.

## Topics

### Getting the Host Information

var host: String

The security origin’s host.

var port: Int

The security origin’s port.

### Getting the Host Protocol

var `protocol`: String

The security origin’s protocol.

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

### Page Content

class WKUserContentController

An object for managing interactions between JavaScript code and your web view, and for filtering content in your web view.

class WKContentRuleListStore

An object that contains the rules for how to load and filter content in the web view.

class WKContentWorld

An object that defines a scope of execution for JavaScript code, and which you use to prevent conflicts between different scripts.

class WKFrameInfo

An object that contains information about a frame on a webpage.

class WKUserScript

A script that the web view injects into a webpage.

