

- Address Book
- ABAddressBook
-  setMe(\_:) 

Instance Method

# setMe(\_:)

Sets the record that represents the logged-in user.

macOS

``` source
func setMe(_ moi: ABPerson!)
```

## Parameters 

`moi`  

The person to set as representing the logged-in user.

## Discussion

If you don’t want a record to represent the logged-in user, then pass `nil` as the `person` argument. Note that this will not delete the existing record, if one is set.

## See Also

### Setting and Retrieving the Logged-in User’s Record

func me() -> ABPerson!

Returns the `ABPerson` record that represents the logged-in user.

