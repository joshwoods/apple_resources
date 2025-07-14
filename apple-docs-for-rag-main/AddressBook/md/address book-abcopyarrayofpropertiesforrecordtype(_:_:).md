

- Address Book
-  ABCopyArrayOfPropertiesForRecordType(\_:\_:) 

Function

# ABCopyArrayOfPropertiesForRecordType(\_:\_:)

Returns an array containing the names of all the properties for the specified record type.

macOS

``` source
func ABCopyArrayOfPropertiesForRecordType(
    _ addressBook: ABAddressBookRef!,
    _ recordType: CFString!
) -> Unmanaged!
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

`recordType`  

Specifies the type of record: kABGroupRecordType or kABPersonRecordType.

## Return Value

An new array containing the names (CFString objects) of all the properties in `recordType`. You are responsible for releasing this object.

## See Also

### Properties

func ABAddPropertiesAndTypes(ABAddressBookRef!, CFString!, CFDictionary!) -> CFIndex

Adds the given properties to all the records of the specified type in the Address Book database, and returns the number of properties successfully added.

func ABCopyLocalizedPropertyOrLabel(CFString!) -> Unmanaged&lt;CFString>!

Returns the localized version of a built in property,label, or key.

func ABLocalizedPropertyOrLabel(String!) -> String!

Returns the localized version of a built in property, label, or key.

func ABRemoveProperties(ABAddressBookRef!, CFString!, CFArray!) -> CFIndex

Removes the given properties from all the records of this type in the Address Book database, and returns the number of properties successfully removed.

func ABTypeOfProperty(ABAddressBookRef!, CFString!, CFString!) -> ABPropertyType

Returns the type of a given property for a given record.

