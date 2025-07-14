

- Address Book
-  ABSearchElementMatchesRecord(\_:\_:) 

Function

# ABSearchElementMatchesRecord(\_:\_:)

Tests whether or not a record matches a search element.

macOS

``` source
func ABSearchElementMatchesRecord(
    _ searchElement: ABSearchElementRef!,
    _ record: ABRecordRef!
) -> Bool
```

## Parameters 

`searchElement`  

The search element containing the query you wish to test `record` with.

`record`  

The record you wish to test.

## Return Value

Returns `true` ifthe `record` parameter satisfies theconditions in the `searchElement`, `false` otherwise.

## See Also

### Search Elements

func ABCopyArrayOfMatchingRecords(ABAddressBookRef!, ABSearchElementRef!) -> Unmanaged&lt;CFArray>!

Returns an array of records that match the given search element, or an empty array if no records match the search element.

func ABSearchElementCreateWithConjunction(ABSearchConjunction, CFArray!) -> Unmanaged&lt;ABSearchElementRef>!

Returns a compound search element created by combiningthe search elements in an array with the given conjunction.

