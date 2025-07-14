

- Foundation
- PersonNameComponents
- PersonNameComponents.FormatStyle
-  init(style:locale:) 

Initializer

# init(style:locale:)

Creates an instance using the provided format style and locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    style: PersonNameComponents.FormatStyle.Style = .medium,
    locale: Locale = .autoupdatingCurrent
)
```

## Parameters 

`style`  

The PersonNameComponents.FormatStyle.Style used to format the name.

`locale`  

The Locale used to create the string representation of the name.

## Discussion

Customize the person name components format style by providing a style and a locale.

The formatted style can be long, medium, short, or abbreviated. The default value is PersonNameComponents.FormatStyle.Style.medium.

The locale provides linguistic and cultural context to the formatted name. The default value is autoupdatingCurrent.

