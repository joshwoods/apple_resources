

- Foundation
- NumberFormatStyleConfiguration
- NumberFormatStyleConfiguration.SignDisplayStrategy
-  automatic 

Type Property

# automatic

A strategy to automatically configure locale-appropriate sign display behavior.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var automatic: NumberFormatStyleConfiguration.SignDisplayStrategy { get }
```

## See Also

### Sign display strategies

static func always(includingZero: Bool) -> NumberFormatStyleConfiguration.SignDisplayStrategy

A strategy to always display sign symbols.

static var never: NumberFormatStyleConfiguration.SignDisplayStrategy

A strategy to never display sign symbols.

