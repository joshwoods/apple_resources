

- Address Book
- ABAddressBook
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes an `ABPerson` or `ABGroup` record from the Address Book database.

macOS

``` source
func remove(_ record: ABRecord!) -> Bool
```

## Parameters 

`record`  

The record to be removed.

## Return Value

`true` if the record was removed successfully; otherwise, `false`.

## Discussion

If `record` is `nil`, this method raises an exception. Your changes are not committed until you call the save() method.

## See Also

### Adding and Removing Records

func add(ABRecord!, error: ()) throws

Adds an `ABPerson` or `ABGroup` record to the Address Book database.

func add(ABRecord!) -> Bool

Adds an `ABPerson` or `ABGroup` record to the Address Book database.

func remove(ABRecord!, error: ()) throws

Removes an `ABPerson` or `ABGroup` record from the Address Book database.

