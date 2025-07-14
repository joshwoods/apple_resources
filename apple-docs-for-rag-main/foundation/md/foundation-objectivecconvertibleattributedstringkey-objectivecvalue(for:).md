

- Foundation
- ObjectiveCConvertibleAttributedStringKey
-  objectiveCValue(for:) 

Type Method

# objectiveCValue(for:)

Returns an Objective-C typed value for a given value of this key’s type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func objectiveCValue(for value: Self.Value) throws -> Self.ObjectiveCValue
```

**Required** Default implementations provided.

## Parameters 

`value`  

The value to convert.

## Return Value

`value`, expressed as the Objective-C type defined by ObjectiveCValue.

## Default Implementations

### ObjectiveCConvertibleAttributedStringKey Implementations

static func objectiveCValue(for: Self.Value) throws -> Self.ObjectiveCValue

static func objectiveCValue(for: Self.Value) throws -> Self.ObjectiveCValue

## See Also

### Converting between Swift and Objective-C Types

static func value(for: Self.ObjectiveCValue) throws -> Self.Value

Returns a value of this key’s type for a given Objective-C value.

**Required** Default implementations provided.

