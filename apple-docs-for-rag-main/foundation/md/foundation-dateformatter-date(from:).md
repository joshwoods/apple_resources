

- Foundation
- DateFormatter
-  date(from:) 

Instance Method

# date(from:)

Returns a date representation of a specified string that the system interprets using the receiver’s current settings.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func date(from string: String) -> Date?
```

## Parameters 

`string`  

The string to parse.

## Return Value

A date representation of `string`. If date(from:) can’t parse the string, returns `nil`.

## Discussion

For more information about using DateFormatter to convert a string to a date, see Working With Fixed Format Date Representations. For a sample code playground, see doc:displaying-human-friendly-content.

## See Also

### Converting Objects

func string(from: Date) -> String

Returns a string representation of a specified date that the system formats using the receiver’s current settings.

class func localizedString(from: Date, dateStyle: DateFormatter.Style, timeStyle: DateFormatter.Style) -> String

Returns a string representation of a specified date, that the system formats for the current locale using the specified date and time styles.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, range: UnsafeMutablePointer&lt;NSRange>?) throws

Returns by reference a date representation of a specified string and its date range, as well as a Boolean value that indicates whether the system can parse the string.

