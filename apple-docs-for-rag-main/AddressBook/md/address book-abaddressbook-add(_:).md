

- Address Book
- ABAddressBook
-  add(\_:) 

Instance Method

# add(\_:)

Adds an `ABPerson` or `ABGroup` record to the Address Book database.

macOS

``` source
func add(_ record: ABRecord!) -> Bool
```

## Parameters 

`record`  

The record to add.

## Return Value

`true` if the record was added successfully; otherwise `false`.

## Discussion

If the `record` argument is `nil`, this method raises an exception. Your changes are not committed until you call the save() method.

It is more efficient to use the ABRecord method init(addressBook:) when possible.

## See Also

### Adding and Removing Records

func add(ABRecord!, error: ()) throws

Adds an `ABPerson` or `ABGroup` record to the Address Book database.

func remove(ABRecord!, error: ()) throws

Removes an `ABPerson` or `ABGroup` record from the Address Book database.

func remove(ABRecord!) -> Bool

Removes an `ABPerson` or `ABGroup` record from the Address Book database.

