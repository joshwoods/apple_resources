

- WebKit
- WKWebExtension
-  WKWebExtension.MatchPattern 

Class

# WKWebExtension.MatchPattern

An object that represents a way to specify groups of URLs.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class MatchPattern
```

## Overview

All match patterns are specified as strings. Apart from the special `` pattern, match patterns consist of three parts: scheme, host, and path.

## Topics

### Errors

struct Error

Constants that indicate errors in the WKWebExtension.MatchPattern domain.

enum Code

Constants that indicate errors in the WKWebExtension.MatchPattern domain.

class let errorDomain: String

A string that identifies the error domain.

### Structures

struct Options

Constants used by WKWebExtension.MatchPattern to indicate matching options.

### Initializers

init(scheme: String, host: String, path: String) throws

Returns a pattern object for the specified scheme, host, and path strings.

init(string: String) throws

Returns a pattern object for the specified pattern string.

### Instance Properties

var host: String?

The host part of the pattern string, unless matchesAllURLs is `YES`.

var matchesAllHosts: Bool

A Boolean value that indicates if the pattern is `` or has `*` as the host.

var matchesAllURLs: Bool

A Boolean value that indicates if the pattern is ``.

var path: String?

The path part of the pattern string, unless matchesAllURLs is `YES`.

var scheme: String?

The scheme part of the pattern string, unless matchesAllURLs is `YES`.

var string: String

The original pattern string.

### Instance Methods

func matches(URL?) -> Bool

Matches the receiver pattern against the specified URL.

func matches(WKWebExtension.MatchPattern?) -> Bool

Matches the receiver pattern against the specified pattern.

func matches(URL?, options: WKWebExtension.MatchPattern.Options) -> Bool

Matches the receiver pattern against the specified URL with options.

func matches(WKWebExtension.MatchPattern?, options: WKWebExtension.MatchPattern.Options) -> Bool

Matches the receiver pattern against the specified pattern with options.

### Type Methods

class func allHostsAndSchemes() -> Self

Returns a pattern object that has `*` for scheme, host, and path.

class func allURLs() -> Self

Returns a pattern object for ``.

class func registerCustomURLScheme(String)

Registers a custom URL scheme that can be used in match patterns.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Classes

class Action

An object that encapsulates the properties for an individual web extension action.

class Command

An object that encapsulates the properties for an individual web extension command.

class DataRecord

An object that represents a record of stored data for a specific web extension context.

class MessagePort

An object that manages message-based communication with a web extension.

class TabConfiguration

An object that encapsulates configuration options for a tab in an extension.

class WindowConfiguration

An object that encapsulates configuration options for a window in an extension.

class Configuration

A WKWebExtensionController.Configuration object with which to initialize a web extension controller.

