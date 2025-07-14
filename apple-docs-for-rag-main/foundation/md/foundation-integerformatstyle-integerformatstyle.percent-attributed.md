

- Foundation
- IntegerFormatStyle
- IntegerFormatStyle.Percent
-  attributed 

Instance Property

# attributed

An attributed format style based on the integer percent format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var attributed: IntegerFormatStyle.Attributed { get }
```

## Discussion

Use this modifier to create an IntegerFormatStyle.Attributed instance, which formats values as AttributedString instances. These attributed strings contain attributes from the AttributeScopes.FoundationAttributes.NumberFormatAttributes attribute scope. Use these attributes to determine which runs of the attributed string represent different parts of the formatted value.

## See Also

### Creating attributed strings

struct Attributed

A format style that converts integers into attributed strings.

