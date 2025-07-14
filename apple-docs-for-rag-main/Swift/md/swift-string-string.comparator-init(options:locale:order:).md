

- Swift
- String
- String.Comparator
-  init(options:locale:order:) 

Initializer

# init(options:locale:order:)

Creates a `String.Comparator` with the given `CompareOptions` and `Locale`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    options: String.CompareOptions,
    locale: Locale? = Locale.current,
    order: SortOrder = .forward
)
```

## Parameters 

`options`  

The options to use for comparison.

`locale`  

The locale to use for comparison. If `nil`, the comparison is unlocalized.

`order`  

The initial order to use for ordered comparison.

