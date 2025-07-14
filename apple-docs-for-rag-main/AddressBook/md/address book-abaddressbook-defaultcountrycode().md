

- Address Book
- ABAddressBook
-  defaultCountryCode() 

Instance Method

# defaultCountryCode()

Returns the default country code for records with unspecified country codes.

macOS 10.3+

``` source
func defaultCountryCode() -> String!
```

## Return Value

The default country code.

## Discussion

This value returned is set by the user in the Address Book application’s general preference. The supported country codes are listed in ABPerson.

## See Also

### Retrieving Default Values

func defaultNameOrdering() -> Int

Returns the default name ordering defined by the user in the Address Book application’s preferences.

