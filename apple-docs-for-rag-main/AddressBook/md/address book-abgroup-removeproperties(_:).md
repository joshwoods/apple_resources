

- Address Book
- ABGroup
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

An array of the properties to be removed.

## Return Value

The number of properties successfully removed.

## Discussion

Only custom properties can be removed. This method is not implemented.

## See Also

### Managing properties

class func addPropertiesAndTypes([AnyHashable : Any]!) -> Int

Adds the given properties to all records of this type in the Address Book database.

class func properties() -> [Any]!

Returns an array of the names of all the properties for this record type in the Address Book database.

class func type(ofProperty: String!) -> ABPropertyType

Returns the type for a given property.

