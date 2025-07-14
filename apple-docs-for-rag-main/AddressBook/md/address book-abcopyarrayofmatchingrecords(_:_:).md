

- Address Book
-  ABCopyArrayOfMatchingRecords(\_:\_:) 

Function

# ABCopyArrayOfMatchingRecords(\_:\_:)

Returns an array of records that match the given search element, or an empty array if no records match the search element.

macOS

``` source
func ABCopyArrayOfMatchingRecords(
    _ addressBook: ABAddressBookRef!,
    _ search: ABSearchElementRef!
) -> Unmanaged!
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

`search`  

The search element that specifies the query. If `search` is `NULL`, this function raises an exception. Create an ABSearchElement object using the record specific functions: ABGroupCreateSearchElement(_:_:_:_:_:) or ABPersonCreateSearchElement(_:_:_:_:_:). See `ABSearchElement C` for more functions that create compound queries.

## Return Value

A new array containing ABRecord objects representing all the records that match `search`. If no records match `search`, this function returns an empty array. You are responsible for releasing this object.

## See Also

### Search Elements

func ABSearchElementCreateWithConjunction(ABSearchConjunction, CFArray!) -> Unmanaged&lt;ABSearchElementRef>!

Returns a compound search element created by combiningthe search elements in an array with the given conjunction.

func ABSearchElementMatchesRecord(ABSearchElementRef!, ABRecordRef!) -> Bool

Tests whether or not a record matches a search element.

