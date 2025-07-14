

- Address Book
-  ABCopyLocalizedPropertyOrLabel(\_:) 

Function

# ABCopyLocalizedPropertyOrLabel(\_:)

Returns the localized version of a built in property,label, or key.

macOS

``` source
func ABCopyLocalizedPropertyOrLabel(_ labelOrProperty: CFString!) -> Unmanaged!
```

## Parameters 

`labelOrProperty`  

The property, label, or key to be localized.

## Return Value

The localized versionof `propertyOrLabel`, or `propertyOrLabel` ifa localized string can not be found. You are responsible for releasingthis object.

## See Also

### Properties

func ABAddPropertiesAndTypes(ABAddressBookRef!, CFString!, CFDictionary!) -> CFIndex

Adds the given properties to all the records of the specified type in the Address Book database, and returns the number of properties successfully added.

func ABCopyArrayOfPropertiesForRecordType(ABAddressBookRef!, CFString!) -> Unmanaged&lt;CFArray>!

Returns an array containing the names of all the properties for the specified record type.

func ABLocalizedPropertyOrLabel(String!) -> String!

Returns the localized version of a built in property, label, or key.

func ABRemoveProperties(ABAddressBookRef!, CFString!, CFArray!) -> CFIndex

Removes the given properties from all the records of this type in the Address Book database, and returns the number of properties successfully removed.

func ABTypeOfProperty(ABAddressBookRef!, CFString!, CFString!) -> ABPropertyType

Returns the type of a given property for a given record.

