

- Foundation
- DateFormatter
-  getObjectValue(\_:for:range:) 

Instance Method

# getObjectValue(\_:for:range:)

Returns by reference a date representation of a specified string and its date range, as well as a Boolean value that indicates whether the system can parse the string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getObjectValue(
    _ obj: AutoreleasingUnsafeMutablePointer?,
    for string: String,
    range rangep: UnsafeMutablePointer?
) throws
```

## Parameters 

`obj`  

If the receiver is able to parse `string`, upon return contains a date representation of `string`.

`string`  

The string to parse.

`rangep`  

If the receiver is able to parse `string`, upon return contains the range of `string` used to create the date.

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func string(for: Any?) -> String?

The default implementation of this method raises an exception.

### Converting Objects

func date(from: String) -> Date?

Returns a date representation of a specified string that the system interprets using the receiver’s current settings.

func string(from: Date) -> String

Returns a string representation of a specified date that the system formats using the receiver’s current settings.

class func localizedString(from: Date, dateStyle: DateFormatter.Style, timeStyle: DateFormatter.Style) -> String

Returns a string representation of a specified date, that the system formats for the current locale using the specified date and time styles.

