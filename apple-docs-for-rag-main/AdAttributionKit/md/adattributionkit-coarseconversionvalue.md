

- AdAttributionKit
-  CoarseConversionValue 

Enumeration

# CoarseConversionValue

Values that describe developer-defined, relative-attribution conversion values.

iOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
enum CoarseConversionValue
```

## Overview

Use these values to differentiate between the value of a person’s actions that are meaningful for a specific interaction. These values have no effect on the framework, but calling the updateConversionValue(_:lockPostback:) method with the value with CoarseConversionValue.low, for example, causes the postback that the ad network receives to have a field `"coarse-conversion-value": "low"`.

## Topics

### Enumeration Cases

case high

A value that represents a developer-defined, coarse conversion value that is high.

case low

A value that represents a developer-defined, coarse conversion value that is low.

case medium

A value that represents a developer-defined, coarse conversion value that is medium.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Postbacks

struct Postback

A structure that provides methods you use to update conversion values for ad attributions.

struct PostbackUpdate

Values you use to update properties in a postback, such as the conversion value.

