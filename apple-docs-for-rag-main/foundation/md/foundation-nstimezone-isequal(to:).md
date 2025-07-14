

- Foundation
- NSTimeZone
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Indicates whether the receiver has the same name and data as the specified time zone.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to aTimeZone: TimeZone) -> Bool
```

## Parameters 

`aTimeZone`  

The time zone to compare with the receiver.

## Return Value

true if `aTimeZone` and the receiver have the same name and data, otherwise false.

