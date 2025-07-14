

- Contacts
- CNPostalAddressFormatter
-  attributedString(from:style:withDefaultAttributes:) 

Type Method

# attributedString(from:style:withDefaultAttributes:)

Returns a postal address as an attributed string and formatted for the specified style.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func attributedString(
    from postalAddress: CNPostalAddress,
    style: CNPostalAddressFormatterStyle,
    withDefaultAttributes attributes: [AnyHashable : Any] = [:]
) -> NSAttributedString
```

## Parameters 

`postalAddress`  

The postal address to format.

`style`  

The postal formatting style to use. For a list of possible values, see CNPostalAddressFormatterStyle.

`attributes`  

The default attributes to use. To learn more, see Formatter.

## Return Value

The formatted postal address as an attributed string.

## Discussion

This method behaves similarly to string(from:), except that it returns an attributed string. It includes the attribute key CNPostalAddressPropertyAttribute, whose attribute values are postal address property keys, such as CNPostalAddressStreetKey. This identifies the postal address components in the formatted postal address. It also includes the attribute key CNPostalAddressLocalizedPropertyNameAttribute whose attribute values are the localized strings for the postal address property keys.

## See Also

### Generating a formatted attributed string

func attributedString(from: CNPostalAddress, withDefaultAttributes: [AnyHashable : Any]) -> NSAttributedString

Returns a formatted postal address as an attributed string.

let CNPostalAddressPropertyAttribute: String

An attribute that identifies the purpose of a range of characters in an attributed string.

let CNPostalAddressLocalizedPropertyNameAttribute: String

An attribute that identifies the localized property of postal address.

