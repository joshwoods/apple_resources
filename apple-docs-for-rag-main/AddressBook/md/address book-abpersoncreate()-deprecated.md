

- Address Book
-  ABPersonCreate() Deprecated

Function

# ABPersonCreate()

Returns a newly created person object.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS

**macOS**

``` source
func ABPersonCreate() -> Unmanaged!
```

**iOS, iPadOS, Mac Catalyst**

``` source
func ABPersonCreate() -> Unmanaged!
```

Deprecated

use \[\[CNMutableContact alloc\] init\]

## Return Value

A newly created person object. You are responsible for releasing this object.

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

func ABPersonCreateSearchElement(CFString!, CFString!, CFString!, CFTypeRef!, ABSearchComparison) -> Unmanaged&lt;ABSearchElementRef>!

Returns a search element object that specifies a query for records of this type.

func ABPersonCreateWithVCardRepresentation(CFData!) -> Unmanaged&lt;ABPersonRef>!

Returns a new ABPerson object initialized with the given data in vCard format.

func ABPersonSetImageData(ABRecord!, CFData!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the image for this person to the given data.

Deprecated

func ABSetMe(ABAddressBookRef!, ABPersonRef!)

Sets the record that represents the logged-in user.

