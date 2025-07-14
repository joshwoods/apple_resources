

- Address Book
- ABGroup
-  addPropertiesAndTypes(\_:) 

Type Method

# addPropertiesAndTypes(\_:)

Adds the given properties to all records of this type in the Address Book database.

macOS

``` source
class func addPropertiesAndTypes(_ properties: [AnyHashable : Any]!) -> Int
```

## Parameters 

`properties`  

A dictionary of properties to be added and their types.

## Return Value

The number of properties successfully added.

## Discussion

In each dictionary entry, the key is a string with the property’s name, and the value is a constant with the property’s type. The property’s name must be unique. You may want to use Java-style package names for your properties, for example, `org.dogclub.dogname` or `com.mycompany.groupID`. The property type must be one of the constants described in Property Types.

## See Also

### Managing properties

class func removeProperties([Any]!) -> Int

Removes the given properties from all the records of this type in the Address Book database.

class func properties() -> [Any]!

Returns an array of the names of all the properties for this record type in the Address Book database.

class func type(ofProperty: String!) -> ABPropertyType

Returns the type for a given property.

