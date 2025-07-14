

- Foundation
- Measurement
- Measurement.FormatStyle
- Measurement.FormatStyle.ByteCount
-  attributed 

Instance Property

# attributed

An attributed format style based on the byte count format style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var attributed: Measurement.AttributedStyle.ByteCount { get }
```

## Discussion

Use this modifier to create a ByteCountFormatStyle.Attributed instance, which formats values as AttributedString instances. These attributed strings contain attributes from the AttributeScopes.FoundationAttributes.NumberFormatAttributes attribute scope. Use these attributes to determine which runs of the attributed string represent different parts of the formatted value.

## See Also

### Creating attributed strings

struct ByteCount

A format style that converts byte counts into attributed strings.

