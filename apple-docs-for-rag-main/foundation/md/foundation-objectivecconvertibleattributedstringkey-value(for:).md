

- Foundation
- ObjectiveCConvertibleAttributedStringKey
-  value(for:) 

Type Method

# value(for:)

Returns a value of this key’s type for a given Objective-C value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func value(for object: Self.ObjectiveCValue) throws -> Self.Value
```

**Required** Default implementations provided.

## Parameters 

`object`  

The Objective-C value to convert.

## Return Value

`object`, expressed as this key’s type.

## Default Implementations

### ObjectiveCConvertibleAttributedStringKey Implementations

static func value(for: Self.ObjectiveCValue) throws -> Self.Value

static func value(for: Self.ObjectiveCValue) throws -> Self.Value

## See Also

### Converting between Swift and Objective-C Types

static func objectiveCValue(for: Self.Value) throws -> Self.ObjectiveCValue

Returns an Objective-C typed value for a given value of this key’s type.

**Required** Default implementations provided.

