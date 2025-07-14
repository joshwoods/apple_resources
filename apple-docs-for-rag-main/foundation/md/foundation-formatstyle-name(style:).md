

- Foundation
- FormatStyle
-  name(style:) 

Type Method

# name(style:)

Returns a format style to use the given name style for formatting a name from its components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func name(style: PersonNameComponents.FormatStyle.Style) -> Self
```

Available when `Self` is `PersonNameComponents.FormatStyle`.

## Parameters 

`style`  

A name-formatting style, such as PersonNameComponents.FormatStyle.Style.long or PersonNameComponents.FormatStyle.Style.abbreviated.

## Return Value

A name format style.

## Discussion

Use the dot-notation form of tis type method when the call point allows the use of PersonNameComponents.FormatStyle. You typically do this when calling the formatted(_:) method of PersonNameComponents.

The following example shows the effect of creating and using different person name format styles.

```
let name = PersonNameComponents(namePrefix: "Dr.",
                                givenName: "Thomas",
                                middleName: "Louis",
                                familyName: "Clark",
                                nameSuffix: "Jr.",
                                nickname: "Tom")
let longFormattedName = name.formatted(.name(style: .long)) // "Dr. Thomas Louis Clark Jr."
let mediumFormattedName = name.formatted(.name(style: .medium)) // "Thomas Clark"
let shortFormattedName = name.formatted(.name(style: .short)) // "Tom"
let abbreviatedFormattedName = name.formatted(.name(style: .abbreviated)) // "TC"
```

