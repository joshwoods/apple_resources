

- Address Book
- ABPerson
-  removeProperties(\_:) 

Type Method

# removeProperties(\_:)

Removes the given properties from all the records of this type in the Address Book database.

macOS

``` source
class func removeProperties(_ properties: [Any]!) -> Int
```

## Parameters 

`properties`  

An array of properties to remove.

## Return Value

The number of properties successfully removed, or `-1` if an error occurs.

## Discussion

Only custom properties can be removed. This method is not implemented.

## See Also

### Managing Properties

class func addPropertiesAndTypes([AnyHashable : Any]!) -> Int

Adds the given properties to all the records of this type in the Address Book database.

class func properties() -> [Any]!

Returns an array of the names of all the properties for the record in the Address Book database.

class func type(ofProperty: String!) -> ABPropertyType

Returns the type of a given property.

