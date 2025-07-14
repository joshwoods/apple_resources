

- Swift
- Duration
- Duration.TimeFormatStyle
-  init(pattern:locale:) 

Initializer

# init(pattern:locale:)

Creates a time format style using the provided pattern and optional locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    pattern: Duration.TimeFormatStyle.Pattern,
    locale: Locale = .autoupdatingCurrent
)
```

## Parameters 

`pattern`  

A `Pattern` that specifies the units to include in the displayed string and the behavior of the units.

`locale`  

The `Locale` used to create the string representation of the duration. This parameter defaults to autoupdatingCurrent.

## See Also

### Creating a time format style

struct Pattern

The units — including hours, minutes, or seconds — and the configuration of those units, used to format a duration.

