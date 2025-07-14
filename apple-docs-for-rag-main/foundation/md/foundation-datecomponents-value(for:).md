

- Foundation
- DateComponents
-  value(for:) 

Instance Method

# value(for:)

Returns the value of one of the properties, using an enumeration value instead of a property name.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(for component: Calendar.Component) -> Int?
```

## Discussion

The calendar and timeZone and isLeapMonth property values cannot be retrieved by this method.

## See Also

### Accessing Calendar Components

func setValue(Int?, for: Calendar.Component)

Set the value of one of the properties, using an enumeration value instead of a property name.

enum Component

An enumeration for the various components of a calendar date.

