

- Foundation
- Locale
-  autoupdatingCurrent 

Type Property

# autoupdatingCurrent

A locale which tracks the user’s current preferences.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var autoupdatingCurrent: Locale { get }
```

## Discussion

If mutated, this Locale will no longer track the user’s preferences.

Note

The autoupdating Locale will only compare equal to another autoupdating Locale.

## See Also

### Getting the user’s locale

static var current: Locale

A locale representing the user’s region settings at the time the property is read.

