

- Address Book
- ABAddressBook
-  formattedAddress(from:) 

Instance Method

# formattedAddress(from:)

Returns an attributed string containing the formatted address.

macOS 10.3+

``` source
func formattedAddress(from address: [AnyHashable : Any]!) -> NSAttributedString!
```

## Parameters 

`address`  

The dictionary containing a street address.

## Return Value

An attributed string containing the formatted address.

## Discussion

The string’s attributes match address dictionary keys, such as `kABAddressStreetKey`. Each attribute value contains the localized description of the key. (For example, the value of a Canadian `kABAddressZIPKey` field would be “Postal Code”, while the value of a French one would be “Code Postal”.)

To get the dictionary containing a street address for a person record, use value(forProperty:) with the property `kABAddressProperty`, and then getting one of the values from the multivalue that is returned.

