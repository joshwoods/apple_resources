

- Address Book
- ABAddressBook
-  groups() 

Instance Method

# groups()

Returns an array of all the groups in the Address Book database.

macOS

``` source
func groups() -> [Any]!
```

## Return Value

An array of all the groups in the Address Book database.

## Discussion

If the database doesn’t contain any groups, this method returns an empty array.

## See Also

### Retrieving Groups and People

func people() -> [Any]!

Returns an array of all the people in the Address Book database.

