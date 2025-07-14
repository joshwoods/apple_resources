

- Scripting Bridge
- SBObject
-  init(properties:) 

Initializer

# init(properties:)

Returns an instance of an `SBObject` subclass initialized with the specified properties.

Mac Catalyst 13.0+macOS 10.5+

``` source
init(properties: [AnyHashable : Any])
```

## Parameters 

`properties`  

A dictionary with keys specifying the names of properties (that is, attributes or to-one relationships) and the values for those properties.

## Return Value

An `SBObject` object or `nil` if the object could not be initialized.

## Discussion

Scripting Bridge does not actually create an object in the target application until you add the object returned from this method to an element array (SBElementArray).

## See Also

### Initializing a Scripting Bridge Object

init()

Initializes and returns an instance of an `SBObject` subclass.

init(data: Any)

Returns an instance of an `SBObject` subclass initialized with the given data.

init(elementCode: DescType, properties: [String : Any]?, data: Any?)

Returns an instance of an `SBObject` subclass initialized with the specified properties and data and added to the designated element array.

