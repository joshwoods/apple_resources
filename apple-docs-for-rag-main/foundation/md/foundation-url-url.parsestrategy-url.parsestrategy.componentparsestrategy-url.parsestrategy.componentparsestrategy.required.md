

- Foundation
- URL
- URL.ParseStrategy
- URL.ParseStrategy.ComponentParseStrategy
-  URL.ParseStrategy.ComponentParseStrategy.required 

Case

# URL.ParseStrategy.ComponentParseStrategy.required

A strategy that requires the presence of the associated component for parsing to succeed.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
case required
```

## See Also

### Component parse strategies

case optional

A strategy that treats the presence of the associated component as optional.

case defaultValue(Component)

A strategy that provides a default value for a component if it’s absent in the source string.

