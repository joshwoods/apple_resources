

- Foundation
- URL
- URL.ParseStrategy
-  URL.ParseStrategy.ComponentParseStrategy 

Enumeration

# URL.ParseStrategy.ComponentParseStrategy

The strategy used to parse one component of a URL.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum ComponentParseStrategy where Component : Decodable, Component : Encodable, Component : Hashable, Component : Sendable
```

## Overview

Use this type with the URL.ParseStrategy initializer and static accessors, or its modifier methods, to specify behavior for parsing components of a URL. This allows you to reject URL candidate strings that lack required components — such as a scheme, host, or path — or to fill in default values while parsing.

## Topics

### Component parse strategies

case required

A strategy that requires the presence of the associated component for parsing to succeed.

case optional

A strategy that treats the presence of the associated component as optional.

case defaultValue(Component)

A strategy that provides a default value for a component if it’s absent in the source string.

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a URL parse strategy

init(scheme: URL.ParseStrategy.ComponentParseStrategy&lt;String>, user: URL.ParseStrategy.ComponentParseStrategy&lt;String>, password: URL.ParseStrategy.ComponentParseStrategy&lt;String>, host: URL.ParseStrategy.ComponentParseStrategy&lt;String>, port: URL.ParseStrategy.ComponentParseStrategy&lt;Int>, path: URL.ParseStrategy.ComponentParseStrategy&lt;String>, query: URL.ParseStrategy.ComponentParseStrategy&lt;String>, fragment: URL.ParseStrategy.ComponentParseStrategy&lt;String>)

Creates a URL parse strategy with the specified component-parsing behaviors.

