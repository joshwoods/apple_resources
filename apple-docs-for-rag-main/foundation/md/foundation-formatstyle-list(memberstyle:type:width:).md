

- Foundation
- FormatStyle
-  list(memberStyle:type:width:) 

Type Method

# list(memberStyle:type:width:)

Returns a format style to format a list of items.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func list(
    memberStyle: MemberStyle,
    type: ListFormatStyle.ListType,
    width: ListFormatStyle.Width = .standard
) -> Self where Self == ListFormatStyle, MemberStyle : FormatStyle, Base : Sequence, MemberStyle.FormatInput == Base.Element, MemberStyle.FormatOutput == String
```

## Parameters 

`memberStyle`  

The format style to apply to each item in the list.

`type`  

The list type to apply, such as cumulative (ListFormatStyle.ListType.and) or alternative (ListFormatStyle.ListType.or) elements.

`width`  

The width to use when formatting, such as ListFormatStyle.Width.standard or ListFormatStyle.Width.narrow.

## Return Value

A list format style that formats an array as a textual list of items.

## Discussion

Use the dot-notation form of this type method when the call point allows the use of ListFormatStyle. You typically do this when calling the formatted(_:) method of Sequence.

The following example creates an array of integers, then uses formatted(_:) and the list format style provided by this method to format the items. By using a currency IntegerFormatStyle, the list format style expresses each member as US dollars. The example also modifies the list format style to use the `en_US` locale, so the resulting string uses US English conventions for commas and conjunctions (“and”).

```
let items: [Int] = [100, 1000, 10000, 100000, 1000000]
let formatted = items.formatted(
    .list(memberStyle: .currency(code: "USD"),
          type: .and)
    .locale(Locale(identifier: "en_US"))) // "$100.00, $1,000.00, $10,000.00, $100,000.00, and $1,000,000.00"
```

## See Also

### Applying list styles

static func list&lt;Base>(type: ListFormatStyle&lt;StringStyle, Base>.ListType, width: ListFormatStyle&lt;StringStyle, Base>.Width) -> Self

Returns a format style to format a list of strings.

