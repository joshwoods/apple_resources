

- Address Book
- ABPerson
-  properties() 

Type Method

# properties()

Returns an array of the names of all the properties for the record in the Address Book database.

macOS

``` source
class func properties() -> [Any]!
```

## See Also

### Managing Properties

class func addPropertiesAndTypes([AnyHashable : Any]!) -> Int

Adds the given properties to all the records of this type in the Address Book database.

class func removeProperties([Any]!) -> Int

Removes the given properties from all the records of this type in the Address Book database.

class func type(ofProperty: String!) -> ABPropertyType

Returns the type of a given property.

