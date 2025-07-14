

- SwiftUI
- LocalizedStringKey
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates a localized string key from the given string interpolation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(stringInterpolation: LocalizedStringKey.StringInterpolation)
```

## Parameters 

`stringInterpolation`  

The string interpolation to use as the localization key.

## Discussion

To create a localized string key from a string interpolation, use the `\()` string interpolation syntax. Swift matches the parameter types in the expression to one of the `appendInterpolation` methods in LocalizedStringKey.StringInterpolation. The interpolated types can include numeric values, Foundation types, and SwiftUI Text and Image instances.

The following example uses a string interpolation with two arguments: an unlabeled Date and a Text.DateStyle labeled `style`. The compiler maps these to the method appendInterpolation(_:style:) as it builds the string that it creates the LocalizedStringKey with.

```
let key = LocalizedStringKey("Date is \(company.foundedDate, style: .offset)")
let text = Text(key) // Text contains "Date is +45 years"
```

You can write this example more concisely, implicitly creating a LocalizedStringKey as the parameter to the Text initializer:

```
let text = Text("Date is \(company.foundedDate, style: .offset)")
```

## See Also

### Creating a key from an interpolation

struct StringInterpolation

Represents the contents of a string literal with interpolations while it’s being built, for use in creating a localized string key.

