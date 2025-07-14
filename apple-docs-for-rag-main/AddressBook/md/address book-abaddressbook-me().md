

- Address Book
- ABAddressBook
-  me() 

Instance Method

# me()

Returns the `ABPerson` record that represents the logged-in user.

macOS

``` source
func me() -> ABPerson!
```

## Return Value

The `ABPerson` record that represents the logged-in user.

## Discussion

If the user never specified such a record, this method returns `nil`.

## See Also

### Setting and Retrieving the Logged-in User’s Record

func setMe(ABPerson!)

Sets the record that represents the logged-in user.

