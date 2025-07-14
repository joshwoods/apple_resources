

- Address Book
- ABAddressBook
-  people() 

Instance Method

# people()

Returns an array of all the people in the Address Book database.

macOS

``` source
func people() -> [Any]!
```

## Return Value

An array of all the people in the Address Book database.

## Discussion

If the database doesn’t contain any people, this method returns an empty array.

## See Also

### Retrieving Groups and People

func groups() -> [Any]!

Returns an array of all the groups in the Address Book database.

