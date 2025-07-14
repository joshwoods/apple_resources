

- Foundation
- ParseableFormatStyle
-  Strategy 

Associated Type

# Strategy

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
associatedtype Strategy : ParseStrategy where Self.FormatInput == Self.Strategy.ParseOutput, Self.FormatOutput == Self.Strategy.ParseInput
```

**Required**

## See Also

### Declaring Parse Strategy

var parseStrategy: Self.Strategy

**Required**

