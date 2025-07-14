

- Foundation
- DateComponentsFormatter
-  string(from:to:) 

Instance Method

# string(from:to:)

Returns a formatted string based on the time difference between two dates.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(
    from startDate: Date,
    to endDate: Date
) -> String?
```

## Parameters 

`startDate`  

The start time. This parameter must not be `nil`.

`endDate`  

The end time. This parameter must not be `nil`.

## Return Value

A formatted string representing the specified time information.

## Discussion

This method calculates the elapsed time between the `startDate` and `endDate` values and uses that information to generate the string. For example, if there is exactly one hour and ten minutes difference between the start and end dates, generating an abbreviated string would result in a string of “1h 10m”.

## See Also

### Formatting Values

func string(from: DateComponents) -> String?

Returns a formatted string based on the specified date component information.

func string(for: Any?) -> String?

Returns a formatted string based on the date information in the specified object.

func string(from: TimeInterval) -> String?

Returns a formatted string based on the specified number of seconds.

class func localizedString(from: DateComponents, unitsStyle: DateComponentsFormatter.UnitsStyle) -> String?

Returns a localized string based on the specified date components and style option.

