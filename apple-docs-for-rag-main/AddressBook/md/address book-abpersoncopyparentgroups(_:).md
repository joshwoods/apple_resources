

- Address Book
-  ABPersonCopyParentGroups(\_:) 

Function

# ABPersonCopyParentGroups(\_:)

Returns an array of groups that a person belongs to.

macOS

``` source
func ABPersonCopyParentGroups(_ person: ABPersonRef!) -> Unmanaged!
```

## Parameters 

`person`  

The person whose parent groups you wish to obtain.

## Return Value

An array of ABGroup objects which `person` belongs to. You are responsible for releasing this object.

## See Also

### People

func ABCopyArrayOfAllPeople(ABAddressBookRef!) -> Unmanaged&lt;CFArray>!

Returns an array of all the people in the Address Book database.

func ABGetMe(ABAddressBookRef!) -> Unmanaged&lt;ABPersonRef>!

Returns the ABPerson object for the logged-in user.

func ABPersonCopyImageData(ABRecord!) -> Unmanaged&lt;CFData>!

Returns data that contains a picture of a person.

Deprecated

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

