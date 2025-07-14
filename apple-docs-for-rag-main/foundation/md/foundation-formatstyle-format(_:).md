

- Foundation
- FormatStyle
-  format(\_:) 

Instance Method

# format(\_:)

Formats a value, using this style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func format(_ value: Self.FormatInput) -> Self.FormatOutput
```

**Required**

## Parameters 

`value`  

The value to format.

## Return Value

A representation of `value`, in the FormatOutput type, formatted according to the style’s configuration.

## Discussion

Use this method when you want to create a single style instance, and then use it to format multiple values.

