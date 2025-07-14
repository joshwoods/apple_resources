

- Address Book
-  ABPersonSetImageData(\_:\_:\_:) Deprecated

Function

# ABPersonSetImageData(\_:\_:\_:)

Sets the image for this person to the given data.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS

**macOS**

``` source
func ABPersonSetImageData(
    _ person: ABPersonRef!,
    _ imageData: CFData!
) -> Bool
```

**iOS, iPadOS, Mac Catalyst**

``` source
func ABPersonSetImageData(
    _ person: ABRecord!,
    _ imageData: CFData!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

Deprecated

use CNMutableContact.imageData

## Parameters 

`person`  

The person whose image data you wish to set.

`imageData`  

The image data to use as the image for `person`.

## Return Value

`true` if successful, `false` otherwise.

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

func ABPersonCreateSearchElement(CFString!, CFString!, CFString!, CFTypeRef!, ABSearchComparison) -> Unmanaged&lt;ABSearchElementRef>!

Returns a search element object that specifies a query for records of this type.

func ABPersonCreateWithVCardRepresentation(CFData!) -> Unmanaged&lt;ABPersonRef>!

Returns a new ABPerson object initialized with the given data in vCard format.

func ABSetMe(ABAddressBookRef!, ABPersonRef!)

Sets the record that represents the logged-in user.

