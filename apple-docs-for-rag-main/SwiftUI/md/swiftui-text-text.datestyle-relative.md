

- SwiftUI
- Text
- Text.DateStyle
-  relative 

Type Property

# relative

A style displaying a date as relative to now.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static let relative: Text.DateStyle
```

## Discussion

```
Text(event.startDate, style: .relative)
```

Example output: 2 hours, 23 minutes 1 year, 1 month

## See Also

### Getting text date styles

static let date: Text.DateStyle

A style displaying a date.

static let offset: Text.DateStyle

A style displaying a date as offset from now.

static let time: Text.DateStyle

A style displaying only the time component for a date.

static let timer: Text.DateStyle

A style displaying a date as timer counting from now.

