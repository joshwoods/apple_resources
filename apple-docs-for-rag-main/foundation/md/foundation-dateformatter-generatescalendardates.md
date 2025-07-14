

- Foundation
- DateFormatter
-  generatesCalendarDates 

Instance Property

# generatesCalendarDates

Indicates whether the formatter generates the deprecated calendar date type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var generatesCalendarDates: Bool { get set }
```

## Discussion

This property is true if the formatter generates the deprecated NSCalendarDate type, and is false otherwise. You should use Date and Calendar rather than NSCalendarDate.

