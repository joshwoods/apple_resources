

- Address Book UI
-  ABCreateStringWithAddressDictionary(\_:\_:) Deprecated

Function

# ABCreateStringWithAddressDictionary(\_:\_:)

Returns a formatted address from an address property.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func ABCreateStringWithAddressDictionary(
    _ address: [AnyHashable : Any],
    _ addCountryName: Bool
) -> String
```

Deprecated

Use CNPostalAddressFormatter instead.

## Parameters 

`address`  

A dictionary representing the address property to format.

`addCountryName`  

Specifies whether to include the name of the country or region in the returned formatted address.

When false and address includes a country or region name, that country or region name is still included in the return value.

When true and `address` doesn’t include a country or region name, the country or region name is added to the return value. (The country or region name is generated from the country code entry in `address`; see `Address Property`.)

## Return Value

The formatted address (may include line endings).

## Discussion

The address is formatted based on the address’s country code (kABPersonAddressCountryCodeKey). In general, the country code should be set to correspond with the country or region name (kABPersonAddressCountryKey).

## See Also

### Detail Display

class ABNewPersonViewController

A view controller presenting an interface to create a contact.

Deprecated

class ABPersonViewController

The `ABPersonViewController` class (whose instances are known as **person view controllers**) implements the view used to display a person record (`ABPersonRef`).

Deprecated

class ABUnknownPersonViewController

The `ABUnknownPersonViewController` class (whose instances are known as **unknown-person view controllers**) implements a view controller used to create a person record from a set of person properties.

Deprecated

