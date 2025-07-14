

- Foundation
- Calendar
-  autoupdatingCurrent 

Type Property

# autoupdatingCurrent

A calendar that tracks changes to user’s preferred calendar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var autoupdatingCurrent: Calendar { get }
```

## Discussion

If mutated, this calendar will no longer track the user’s preferred calendar.

Note

The autoupdating Calendar will only compare equal to another autoupdating Calendar.

## See Also

### Getting the User’s Calendar

static var current: Calendar

The user’s current calendar.

