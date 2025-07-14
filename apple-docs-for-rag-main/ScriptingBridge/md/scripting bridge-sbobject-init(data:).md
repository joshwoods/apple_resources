

- Scripting Bridge
- SBObject
-  init(data:) 

Initializer

# init(data:)

Returns an instance of an `SBObject` subclass initialized with the given data.

Mac Catalyst 13.0+macOS 10.5+

``` source
init(data: Any)
```

## Parameters 

`data`  

An object containing data for the new `SBObject` object. The data varies according to the type of scripting object to be created.

## Return Value

An `SBObject` object or `nil` if the object could not be initialized.

## Discussion

Scripting Bridge does not actually create an object in the target application until you add the object returned from this method to an element array (SBElementArray).

## See Also

### Initializing a Scripting Bridge Object

init()

Initializes and returns an instance of an `SBObject` subclass.

init(properties: [AnyHashable : Any])

Returns an instance of an `SBObject` subclass initialized with the specified properties.

init(elementCode: DescType, properties: [String : Any]?, data: Any?)

Returns an instance of an `SBObject` subclass initialized with the specified properties and data and added to the designated element array.

