

- Accessibility
- AXDataSeriesDescriptor
-  attributedName 

Instance Property

# attributedName

An attributed version of the data series name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@NSCopying
var attributedName: NSAttributedString { get set }
```

## Discussion

If you set the value of this property, the system uses this value instead of name.

## See Also

### Naming the series

var name: String?

The name of the data series.

