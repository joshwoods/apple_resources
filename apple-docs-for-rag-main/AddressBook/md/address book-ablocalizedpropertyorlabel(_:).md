

- Address Book
-  ABLocalizedPropertyOrLabel(\_:) 

Function

# ABLocalizedPropertyOrLabel(\_:)

Returns the localized version of a built in property, label, or key.

macOS

``` source
func ABLocalizedPropertyOrLabel(_ propertyOrLabel: String!) -> String!
```

## Discussion

The `propertyOrLabel` argument is the property, label, or key you wish to localize. Returns `propertyOrLabel` if a localized string can not be found

## See Also

### Properties

func ABAddPropertiesAndTypes(ABAddressBookRef!, CFString!, CFDictionary!) -> CFIndex

Adds the given properties to all the records of the specified type in the Address Book database, and returns the number of properties successfully added.

func ABCopyArrayOfPropertiesForRecordType(ABAddressBookRef!, CFString!) -> Unmanaged&lt;CFArray>!

Returns an array containing the names of all the properties for the specified record type.

func ABCopyLocalizedPropertyOrLabel(CFString!) -> Unmanaged&lt;CFString>!

Returns the localized version of a built in property,label, or key.

func ABRemoveProperties(ABAddressBookRef!, CFString!, CFArray!) -> CFIndex

Removes the given properties from all the records of this type in the Address Book database, and returns the number of properties successfully removed.

func ABTypeOfProperty(ABAddressBookRef!, CFString!, CFString!) -> ABPropertyType

Returns the type of a given property for a given record.

