

- Foundation
- ISO8601DateFormatter
-  timeZone 

Instance Property

# timeZone

The time zone used to create and parse date representations. When unspecified, GMT is used.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var timeZone: TimeZone! { get set }
```

## Discussion

Resetting this property can incur a significant performance cost, as it may cause internal state to be regenerated.

## See Also

### Configuring the Formatter

var formatOptions: ISO8601DateFormatter.Options

Options for generating and parsing ISO 8601 date representations. See ISO8601DateFormatter.Options for possible values.

