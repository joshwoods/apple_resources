

- Contacts
- CNPostalAddressFormatter
-  string(from:) 

Instance Method

# string(from:)

Returns a formatted postal address.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func string(from postalAddress: CNPostalAddress) -> String
```

## Parameters 

`postalAddress`  

The postal address to format.

## Return Value

The formatted postal address.

## See Also

### Generating a formatted string

class func string(from: CNPostalAddress, style: CNPostalAddressFormatterStyle) -> String

Returns a postal address as a string and formatted for the specified style.

