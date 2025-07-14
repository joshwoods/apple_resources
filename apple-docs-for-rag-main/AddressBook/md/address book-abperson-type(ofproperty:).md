

- Address Book
- ABPerson
-  type(ofProperty:) 

Type Method

# type(ofProperty:)

Returns the type of a given property.

macOS

``` source
class func type(ofProperty property: String!) -> ABPropertyType
```

## Parameters 

`property`  

The property whose type will be returned.

## Discussion

If the property does not exist, this method returns `kABErrorInProperty`.

## See Also

### Managing Properties

class func addPropertiesAndTypes([AnyHashable : Any]!) -> Int

Adds the given properties to all the records of this type in the Address Book database.

class func removeProperties([Any]!) -> Int

Removes the given properties from all the records of this type in the Address Book database.

class func properties() -> [Any]!

Returns an array of the names of all the properties for the record in the Address Book database.

