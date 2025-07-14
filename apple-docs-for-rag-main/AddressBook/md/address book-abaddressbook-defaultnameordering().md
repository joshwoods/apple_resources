

- Address Book
- ABAddressBook
-  defaultNameOrdering() 

Instance Method

# defaultNameOrdering()

Returns the default name ordering defined by the user in the Address Book application’s preferences.

macOS 10.3+

``` source
func defaultNameOrdering() -> Int
```

## Return Value

The default name ordering defined by the user in the Address Book application’s preferences.

## Discussion

The possible values are kABFirstNameFirst and kABLastNameFirst.

## See Also

### Retrieving Default Values

func defaultCountryCode() -> String!

Returns the default country code for records with unspecified country codes.

