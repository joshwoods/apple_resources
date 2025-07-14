

- Address Book
-  ABAddPropertiesAndTypes(\_:\_:\_:) 

Function

# ABAddPropertiesAndTypes(\_:\_:\_:)

Adds the given properties to all the records of the specified type in the Address Book database, and returns the number of properties successfully added.

macOS

``` source
func ABAddPropertiesAndTypes(
    _ addressBook: ABAddressBookRef!,
    _ recordType: CFString!,
    _ propertiesAndTypes: CFDictionary!
) -> CFIndex
```

## Parameters 

`addressBook`  

The address book for the logged-in user.

`recordType`  

The record type you wish to add properties to: kABGroupRecordType or kABPersonRecordType.

`propertiesAndTypes`  

A CFDictionary object containing the properties to add. In each dictionary entry, the key is a string with the property’s name, and the value is a constant with the property’s type. The property’s name must be unique. You may want to use Java-style package names for your properties, for example, `"org.dogclub.dogname"` or `"com.mycompany.customerID"`. The property type must be one of the constants described in ABPropertyType.

## Return Value

The number of properties successfully added.

## See Also

### Properties

func ABCopyArrayOfPropertiesForRecordType(ABAddressBookRef!, CFString!) -> Unmanaged&lt;CFArray>!

Returns an array containing the names of all the properties for the specified record type.

func ABCopyLocalizedPropertyOrLabel(CFString!) -> Unmanaged&lt;CFString>!

Returns the localized version of a built in property,label, or key.

func ABLocalizedPropertyOrLabel(String!) -> String!

Returns the localized version of a built in property, label, or key.

func ABRemoveProperties(ABAddressBookRef!, CFString!, CFArray!) -> CFIndex

Removes the given properties from all the records of this type in the Address Book database, and returns the number of properties successfully removed.

func ABTypeOfProperty(ABAddressBookRef!, CFString!, CFString!) -> ABPropertyType

Returns the type of a given property for a given record.

