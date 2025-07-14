

- Address Book
-  ABPersonCreateSearchElement(\_:\_:\_:\_:\_:) 

Function

# ABPersonCreateSearchElement(\_:\_:\_:\_:\_:)

Returns a search element object that specifies a query for records of this type.

macOS

``` source
func ABPersonCreateSearchElement(
    _ property: CFString!,
    _ label: CFString!,
    _ key: CFString!,
    _ value: CFTypeRef!,
    _ comparison: ABSearchComparison
) -> Unmanaged!
```

## Parameters 

`property`  

The name of the property to search on. It cannot be `NULL`. For a full list of the properties, see `Person Properties` and Common Properties in ABRecord.

`label`  

The label name for a multi-value list. If `property` does not have multiple values, pass `NULL`. If `property` does have multiple values, pass `NULL` to search all the values.

`key`  

The key name for a dictionary. If `property` is not a dictionary, pass `NULL`. If `property` is a dictionary, pass `NULL` to search all keys.

`value`  

The value you are searching for. It cannot be `NULL`

`comparison`  

Specifies the type of comparison to perform, such as kABEqual or kABPrefixMatchCaseInsensitive. For a full list, see ABSearchComparison.

## Return Value

A search element object that specifies a query according to the above parameters. You are responsible for releasing this object.

## Discussion

Use the ABAddressBook ABCopyArrayOfMatchingRecords(_:_:) function to actually perform the query. Also, see `ABSearchElement C` for more functions that create compound queries.

## See Also

### People

func ABCopyArrayOfAllPeople(ABAddressBookRef!) -> Unmanaged&lt;CFArray>!

Returns an array of all the people in the Address Book database.

func ABGetMe(ABAddressBookRef!) -> Unmanaged&lt;ABPersonRef>!

Returns the ABPerson object for the logged-in user.

func ABPersonCopyImageData(ABRecord!) -> Unmanaged&lt;CFData>!

Returns data that contains a picture of a person.

Deprecated

func ABPersonCopyParentGroups(ABPersonRef!) -> Unmanaged&lt;CFArray>!

Returns an array of groups that a person belongs to.

func ABPersonCopyVCardRepresentation(ABPersonRef!) -> Unmanaged&lt;CFData>!

Returns the vCard representation of the person as a data object in vCard format.

func ABPersonCreate() -> Unmanaged&lt;ABRecord>!

Returns a newly created person object.

Deprecated

func ABPersonCreateWithVCardRepresentation(CFData!) -> Unmanaged&lt;ABPersonRef>!

Returns a new ABPerson object initialized with the given data in vCard format.

func ABPersonSetImageData(ABRecord!, CFData!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the image for this person to the given data.

Deprecated

func ABSetMe(ABAddressBookRef!, ABPersonRef!)

Sets the record that represents the logged-in user.

