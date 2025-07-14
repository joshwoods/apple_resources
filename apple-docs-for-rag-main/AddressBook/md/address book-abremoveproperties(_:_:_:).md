

- Address Book
-  ABRemoveProperties(\_:\_:\_:) 

Function

# ABRemoveProperties(\_:\_:\_:)

Removes the given properties from all the records of this type in the Address Book database, and returns the number of properties successfully removed.

macOS

``` source
func ABRemoveProperties(
    _ addressBook: ABAddressBookRef!,
    _ recordType: CFString!,
    _ properties: CFArray!
) -> CFIndex
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

`recordType`  

The name of record to remove the properties from: kABGroupRecordType or kABPersonRecordType.

`properties`  

An array of properties (CFString objects) to remove.

## Return Value

The number of properties successfully removed.

## Discussion

Only custom properties can be removed. This function is not implemented.

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

func ABTypeOfProperty(ABAddressBookRef!, CFString!, CFString!) -> ABPropertyType

Returns the type of a given property for a given record.

