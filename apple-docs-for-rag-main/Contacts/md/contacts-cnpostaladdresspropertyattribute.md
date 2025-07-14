

- Contacts
-  CNPostalAddressPropertyAttribute 

Global Variable

# CNPostalAddressPropertyAttribute

An attribute that identifies the purpose of a range of characters in an attributed string.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
let CNPostalAddressPropertyAttribute: String
```

## Discussion

The value of this key is a string constant that specifies the meaning of the range of characters. For example, the value is CNPostalAddressCityKey when the characters specify the city portion of the address.

## See Also

### Generating a formatted attributed string

func attributedString(from: CNPostalAddress, withDefaultAttributes: [AnyHashable : Any]) -> NSAttributedString

Returns a formatted postal address as an attributed string.

class func attributedString(from: CNPostalAddress, style: CNPostalAddressFormatterStyle, withDefaultAttributes: [AnyHashable : Any]) -> NSAttributedString

Returns a postal address as an attributed string and formatted for the specified style.

let CNPostalAddressLocalizedPropertyNameAttribute: String

An attribute that identifies the localized property of postal address.

