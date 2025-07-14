

- Foundation
- NSScriptClassDescription
-  init(for:) 

Initializer

# init(for:)

Returns the class description for the specified class or, if it is not scriptable, for the first superclass that is.

Mac Catalyst 13.0+macOS 10.0+

``` source
init?(for aClass: AnyClass)
```

## Parameters 

`aClass`  

The class whose description is needed.

## Return Value

The class description for the class specified by `aClass` or, if that class isn’t scriptable, for the class description for the first superclass that is. Returns `nil` if it doesn’t find a scriptable class.

## See Also

### Getting a Script Class Description

func forKey(String) -> NSScriptClassDescription?

Returns the class description instance for the class type of the specified attribute or relationship.

var superclass: NSScriptClassDescription?

Returns the class description instance for the superclass of the receiver’s class.

