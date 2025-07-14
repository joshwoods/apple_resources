

- Scripting Bridge
- SBObject
-  init(elementCode:properties:data:) 

Initializer

# init(elementCode:properties:data:)

Returns an instance of an `SBObject` subclass initialized with the specified properties and data and added to the designated element array.

Mac Catalyst 13.0+macOS 10.5+

``` source
init(
    elementCode code: DescType,
    properties: [String : Any]?,
    data: Any?
)
```

## Parameters 

`code`  

A four-character code used to identify an element in the target application’s scripting interface. See Apple Event Manager for details.

`properties`  

A dictionary with NSNumber keys specifying the four-character codes of properties (that is, attributes or to-one relationships) and the values for those properties. Pass `nil` if you are initializing the object by `data` only.

`data`  

An object containing data for the new `SBObject` object. The data varies according to the type of scripting object to be created. Pass `nil` if you initializing the object by `properties` only.

## Return Value

An `SBObject` object or `nil` if the object could not be initialized.

## Discussion

Unlike the other initializers of this class, this method not only initializes the `SBObject` object but adds it to a specified element array. This method is the designated initializer.

## See Also

### Initializing a Scripting Bridge Object

init()

Initializes and returns an instance of an `SBObject` subclass.

init(data: Any)

Returns an instance of an `SBObject` subclass initialized with the given data.

init(properties: [AnyHashable : Any])

Returns an instance of an `SBObject` subclass initialized with the specified properties.

