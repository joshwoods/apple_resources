

- Foundation
- DateComponentsFormatter
-  string(for:) 

Instance Method

# string(for:)

Returns a formatted string based on the date information in the specified object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(for obj: Any?) -> String?
```

## Parameters 

`obj`  

An object containing the date and time information to format. The object in this parameter must be a NSDateComponents object; if it is not, the method raises an exception. This parameter must not be `nil`.

## Return Value

A formatted string representing the specified date information.

## Discussion

This method has the same behavior as the string(from:) method.

## See Also

### Formatting Values

func string(from: DateComponents) -> String?

Returns a formatted string based on the specified date component information.

func string(from: Date, to: Date) -> String?

Returns a formatted string based on the time difference between two dates.

func string(from: TimeInterval) -> String?

Returns a formatted string based on the specified number of seconds.

class func localizedString(from: DateComponents, unitsStyle: DateComponentsFormatter.UnitsStyle) -> String?

Returns a localized string based on the specified date components and style option.

