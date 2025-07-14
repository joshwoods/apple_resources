

- Foundation
- DateComponents
-  setValue(\_:for:) 

Instance Method

# setValue(\_:for:)

Set the value of one of the properties, using an enumeration value instead of a property name.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func setValue(
    _ value: Int?,
    for component: Calendar.Component
)
```

## Discussion

The calendar and timeZone and isLeapMonth properties cannot be set by this method.

## See Also

### Accessing Calendar Components

func value(for: Calendar.Component) -> Int?

Returns the value of one of the properties, using an enumeration value instead of a property name.

enum Component

An enumeration for the various components of a calendar date.

