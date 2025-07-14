

- Address Book
-  ABTypeOfProperty(\_:\_:\_:) 

Function

# ABTypeOfProperty(\_:\_:\_:)

Returns the type of a given property for a given record.

macOS

``` source
func ABTypeOfProperty(
    _ addressBook: ABAddressBookRef!,
    _ recordType: CFString!,
    _ property: CFString!
) -> ABPropertyType
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

`recordType`  

The record type that contains `property`: kABGroupRecordType or kABPersonRecordType.

`property`  

The property whose type you wish to obtain.

## Return Value

The type of `property` as defined in ABPropertyType. If `property` does not exist in `recordType`, this function returns kABErrorInProperty.

## See Also

### Properties

func ABAddPropertiesAndTypes(ABAddressBookRef!, CFString!, CFDictionary!) -> CFIndex

Adds the given properties to all the records of the specified type in the Address Book database, and returns the number of properties successfully added.

func ABCopyArrayOfPropertiesForRecordType(ABAddressBookRef!, CFString!) -> Unmanaged&lt;CFArray>!

Returns an array containing the names of all the properties for the specified record type.

func ABCopyLocalizedPropertyOrLabel(CFString!) -> Unmanaged&lt;CFString>!

Returns the localized version of a built in property,label, or key.

func ABLocalizedPropertyOrLabel(String!) -> String!

Returns the localized version of a built in property, label, or key.

func ABRemoveProperties(ABAddressBookRef!, CFString!, CFArray!) -> CFIndex

Removes the given properties from all the records of this type in the Address Book database, and returns the number of properties successfully removed.

