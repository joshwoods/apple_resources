

- Address Book
-  ABGetMe(\_:) 

Function

# ABGetMe(\_:)

Returns the ABPerson object for the logged-in user.

macOS

``` source
func ABGetMe(_ addressBook: ABAddressBookRef!) -> Unmanaged!
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

## Return Value

The ABPerson record that represents the logged-in user, or `NULL` if the user never specified such a record. You are responsible for retaining and releasing this object as needed.

## See Also

### People

func ABCopyArrayOfAllPeople(ABAddressBookRef!) -> Unmanaged&lt;CFArray>!

Returns an array of all the people in the Address Book database.

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

func ABPersonCreateSearchElement(CFString!, CFString!, CFString!, CFTypeRef!, ABSearchComparison) -> Unmanaged&lt;ABSearchElementRef>!

Returns a search element object that specifies a query for records of this type.

func ABPersonCreateWithVCardRepresentation(CFData!) -> Unmanaged&lt;ABPersonRef>!

Returns a new ABPerson object initialized with the given data in vCard format.

func ABPersonSetImageData(ABRecord!, CFData!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the image for this person to the given data.

Deprecated

func ABSetMe(ABAddressBookRef!, ABPersonRef!)

Sets the record that represents the logged-in user.

