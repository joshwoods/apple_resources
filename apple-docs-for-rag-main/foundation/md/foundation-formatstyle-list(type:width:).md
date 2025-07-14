

- Foundation
- FormatStyle
-  list(type:width:) 

Type Method

# list(type:width:)

Returns a format style to format a list of strings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func list(
    type: ListFormatStyle.ListType,
    width: ListFormatStyle.Width = .standard
) -> Self where Self == ListFormatStyle, Base : Sequence, Base.Element == String
```

## Parameters 

`type`  

The list type to apply, such as cumulative (ListFormatStyle.ListType.and) or alternative (ListFormatStyle.ListType.or) elements.

`width`  

The width to use when formatting, such as ListFormatStyle.Width.standard or ListFormatStyle.Width.narrow.

## Return Value

A list format style that formats a string array as a textual list of items.

## Discussion

Use the dot-notation form of this type method when the call point allows the use of ListFormatStyle, and the Sequence element type is String. You typically do this when calling the formatted(_:) method of Sequence.

The following example creates an array of strings, then uses formatted(_:) and the list format style provided by this method to format the items. It modifies the list format style to use the `en_US` locale, so the resulting string uses US English conventions for commas and conjunctions (“and”).

```
let items = ["Atlantic", "Pacific", "Indian", "Arctic", "Southern"]
let formatted = items.formatted(
    .list(type:.and)
    .locale(Locale(identifier: "en_US"))) // "Atlantic, Pacific, Indian, Arctic, and Southern"
```

## See Also

### Applying list styles

static func list&lt;MemberStyle, Base>(memberStyle: MemberStyle, type: ListFormatStyle&lt;MemberStyle, Base>.ListType, width: ListFormatStyle&lt;MemberStyle, Base>.Width) -> Self

Returns a format style to format a list of items.

