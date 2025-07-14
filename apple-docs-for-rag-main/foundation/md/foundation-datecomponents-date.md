

- Foundation
- DateComponents
-  date 

Instance Property

# date

The date calculated from the current components using the stored calendar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var date: Date? { get }
```

## See Also

### Validating a Date

var isValidDate: Bool

Indicates whether the current combination of properties represents a date which exists in the current calendar.

func isValidDate(in: Calendar) -> Bool

Indicates whether the current combination of properties represents a date which exists in the specified calendar.

