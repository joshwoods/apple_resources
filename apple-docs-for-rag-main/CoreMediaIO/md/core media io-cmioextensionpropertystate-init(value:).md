

- Core Media I/O
- CMIOExtensionPropertyState
-  init(value:) 

Initializer

# init(value:)

Creates a property state with a value.

Mac Catalyst 15.4+macOS 12.3+

``` source
convenience init(value: ObjectType?)
```

## Parameters 

`value`  

The value to associate with the property state.

## Discussion

The system supports the following value types: NSDictionary, NSArray, NSString, NSData, and NSNumber.

## See Also

### Creating a Property State

init(value: ObjectType?, attributes: CMIOExtensionPropertyAttributes&lt;ObjectType>?)

Creates a property state with a value and attributes.

