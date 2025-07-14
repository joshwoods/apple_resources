

- Swift
- String
- String.LocalizationValue
-  init(\_:) 

Initializer

# init(\_:)

Creates a localization value instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(_ value: String)
```

## Parameters 

`value`  

A string that provides the localization key to look up. This parameter also serves as the default value if the system can’t find a localized string.

## Discussion

Creating a String.LocalizationValue with this initializer creates a localized value with no interpolated values.

