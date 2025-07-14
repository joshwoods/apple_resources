

- XPC
- XPCDictionary
-  init(\_:) 

Initializer

# init(\_:)

Creates a dictionary using the keys and values in the specified object parameter.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
init(_ value: xpc_object_t)
```

## Parameters 

`value`  

An XPC dictionary object. The object’s type must be XPC_TYPE_DICTIONARY.

## See Also

### Creating a dictionary

init()

Creates an empty dictionary.

func copy(into: XPCDictionary)

Copies the keys and values of the dictionary to a different dictionary.

