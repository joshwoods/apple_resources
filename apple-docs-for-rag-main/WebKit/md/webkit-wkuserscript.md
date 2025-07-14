

- WebKit
-  WKUserScript 

Class

# WKUserScript

A script that the web view injects into a webpage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKUserScript
```

## Overview

Create a WKUserScript object when you want to inject custom script code into the pages of your web view. Use this object to specify the JavaScript code to inject, and parameters relating to when and how to inject that code. Before you create the web view, add this object to the WKUserContentController object associated with your web view’s configuration.

## Topics

### Creating a User Script Object

init(source: String, injectionTime: WKUserScriptInjectionTime, forMainFrameOnly: Bool)

Creates a user script object that contains the specified source code and attributes.

init(source: String, injectionTime: WKUserScriptInjectionTime, forMainFrameOnly: Bool, in: WKContentWorld)

Creates a user script object that is scoped to a particular content world.

### Inspecting Script Information

var source: String

The script’s source code.

var injectionTime: WKUserScriptInjectionTime

The time at which to inject the script into the webpage.

enum WKUserScriptInjectionTime

Constants for the times at which to inject script content into a webpage.

var isForMainFrameOnly: Bool

A Boolean value that indicates whether to inject the script into the main frame or all frames.

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

class WKFrameInfo

An object that contains information about a frame on a webpage.

class WKSecurityOrigin

An object that identifies the origin of a particular resource.

