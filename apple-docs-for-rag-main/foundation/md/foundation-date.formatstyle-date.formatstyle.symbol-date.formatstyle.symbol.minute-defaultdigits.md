

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Minute
-  defaultDigits 

Type Property

# defaultDigits

The custom minute format style showing the minimum number of digits that represents the numeric minute.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var defaultDigits: Date.FormatStyle.Symbol.Minute { get }
```

## Discussion

For example, this style represents one minute past the hour as `1`, and eighteen past as `18`.

## See Also

### Modifying a Minute

static var twoDigits: Date.FormatStyle.Symbol.Minute

The custom format style that shows the two-digit numeric minute, zero-padded if necessary.

