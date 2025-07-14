

- Foundation
- URL
- URL.FormatStyle
-  URL.FormatStyle.Component 

Enumeration

# URL.FormatStyle.Component

An enumeration of the components of a URL, for use in creating format style options that depend on a component’s value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Component
```

## Overview

You use this type with style-modifying methods like displayWhen(_:matches:) in URL.FormatStyle.ComponentDisplayOption and omitWhen(_:matches:) in URL.FormatStyle.HostDisplayOption.

## Topics

### URL format style components

case scheme

The URL format style scheme component.

case host

The URL format style host component.

case port

The URL format style port component.

case user

The URL format style user component.

case password

The URL format style password component.

case path

The URL format style path component.

case query

The URL format style query component.

case fragment

The URL format style fragment component.

### Comparing URL format style components

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Display options

static var always: URL.FormatStyle.ComponentDisplayOption

A display option that always displays the component.

static var never: URL.FormatStyle.ComponentDisplayOption

A display option that never displays the component.

static var omitIfHTTPFamily: URL.FormatStyle.ComponentDisplayOption

A display option that omits the component if the URL scheme is any flavor of HTTP.

static func displayWhen(URL.FormatStyle.Component, matches: Set&lt;String>) -> URL.FormatStyle.ComponentDisplayOption

Returns a display option that displays the component when a specified component meets the specified requirements.

static func omitWhen(URL.FormatStyle.Component, matches: Set&lt;String>) -> URL.FormatStyle.ComponentDisplayOption

Returns a display option that omits the component when a specified component meets the specified requirements.

