

- Foundation
- DateComponentsFormatter
-  string(from:) 

Instance Method

# string(from:)

Returns a formatted string based on the specified date component information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(from components: DateComponents) -> String?
```

## Parameters 

`components`  

A date components object containing the date and time information to format. The allowedUnits property determines which date components are actually used to generate the string. All other date components are ignored. This parameter must not be `nil`.

## Return Value

A formatted string representing the specified date information.

## Discussion

Use this method to format date information that is already broken down into the component day and time values.

## See Also

### Formatting Values

func string(for: Any?) -> String?

Returns a formatted string based on the date information in the specified object.

func string(from: Date, to: Date) -> String?

Returns a formatted string based on the time difference between two dates.

func string(from: TimeInterval) -> String?

Returns a formatted string based on the specified number of seconds.

class func localizedString(from: DateComponents, unitsStyle: DateComponentsFormatter.UnitsStyle) -> String?

Returns a localized string based on the specified date components and style option.

