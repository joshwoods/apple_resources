

- Address Book
-  ABSearchElementCreateWithConjunction(\_:\_:) 

Function

# ABSearchElementCreateWithConjunction(\_:\_:)

Returns a compound search element created by combiningthe search elements in an array with the given conjunction.

macOS

``` source
func ABSearchElementCreateWithConjunction(
    _ conjunction: ABSearchConjunction,
    _ childrenSearchElement: CFArray!
) -> Unmanaged!
```

## Parameters 

`conjunction`  

The conjunction used to join the search elements in `children`. Can be either kABSearchAnd or kABSearchOr.

`childrenSearchElement`  

An array containing ABSearchElement objects to be joined using `conjunction`. If `NULL` this function raises an exception.

## Return Value

A new compound searchelement joining the search elements in `children` using `conjunction`.You are responsible for releasing this object.

## See Also

### Search Elements

func ABCopyArrayOfMatchingRecords(ABAddressBookRef!, ABSearchElementRef!) -> Unmanaged&lt;CFArray>!

Returns an array of records that match the given search element, or an empty array if no records match the search element.

func ABSearchElementMatchesRecord(ABSearchElementRef!, ABRecordRef!) -> Bool

Tests whether or not a record matches a search element.

