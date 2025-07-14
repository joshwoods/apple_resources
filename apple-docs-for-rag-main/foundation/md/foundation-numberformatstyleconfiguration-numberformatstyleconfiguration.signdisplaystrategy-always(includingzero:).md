

- Foundation
- NumberFormatStyleConfiguration
- NumberFormatStyleConfiguration.SignDisplayStrategy
-  always(includingZero:) 

Type Method

# always(includingZero:)

A strategy to always display sign symbols.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func always(includingZero: Bool = true) -> NumberFormatStyleConfiguration.SignDisplayStrategy
```

## Parameters 

`includingZero`  

A Boolean value that determines whether the format style should apply sign characters to zero values. Defaults to `true`.

## Return Value

A strategy to always display sign symbols, with the given behavior for zero values.

## See Also

### Sign display strategies

static var automatic: NumberFormatStyleConfiguration.SignDisplayStrategy

A strategy to automatically configure locale-appropriate sign display behavior.

static var never: NumberFormatStyleConfiguration.SignDisplayStrategy

A strategy to never display sign symbols.

