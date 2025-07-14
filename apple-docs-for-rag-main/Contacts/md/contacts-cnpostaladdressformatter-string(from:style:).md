

- Contacts
- CNPostalAddressFormatter
-  string(from:style:) 

Type Method

# string(from:style:)

Returns a postal address as a string and formatted for the specified style.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func string(
    from postalAddress: CNPostalAddress,
    style: CNPostalAddressFormatterStyle
) -> String
```

## Parameters 

`postalAddress`  

The postal address to format.

`style`  

The postal formatting style to use. For a list of possible values, see CNPostalAddressFormatterStyle.

## Return Value

The formatted postal address.

## See Also

### Generating a formatted string

func string(from: CNPostalAddress) -> String

Returns a formatted postal address.

