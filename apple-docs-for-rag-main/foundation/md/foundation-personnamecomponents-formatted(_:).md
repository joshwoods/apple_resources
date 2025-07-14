

- Foundation
- PersonNameComponents
-  formatted(\_:) 

Instance Method

# formatted(\_:)

Generates a locale-aware string representation of an instance of person name components using the provided format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formatted(_ style: S) -> S.FormatOutput where S : FormatStyle, S.FormatInput == PersonNameComponents
```

## Parameters 

`style`  

Specifies the PersonNameComponents.FormatStyle applied to the person name components.

## Return Value

A string, formatted according to the provided style.

## Discussion

Use the formatted(_:) method to create a string representation of a person’s name with a customized length for specific uses. You can use the PersonNameComponents.FormatStyle static factory method `PersonNameComponents/FormatStyle/name(style:)-6tpu3` to create a custom format style as a parameter to the method.

For example:

```
var tlc = PersonNameComponents()
tlc.familyName = "Clark"
tlc.givenName = "Thomas"
tlc.middleName = "Louis"
tlc.namePrefix = "Dr."
tlc.nickname = "Tom"
tlc.nameSuffix = "Esq."

tlc.formatted(.name(style: .long))
// Dr. Thomas Louis Clark Esq.

tlc.formatted(.name(style: .medium))
// Thomas Clark

tlc.formatted(.name(style: .short))
// Tom

tlc.formatted(.name(style: .abbreviated))
// TC
```

## See Also

### Formatting Person Name Components

func formatted() -> String

Generates a locale-aware string representation of an instance of person name components using the default format style.

struct FormatStyle

A type used to format a person’s name with a style appropriate for the given locale.

