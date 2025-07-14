

- Foundation
- NSScriptClassDescription
-  forKey(\_:) 

Instance Method

# forKey(\_:)

Returns the class description instance for the class type of the specified attribute or relationship.

Mac Catalyst 13.0+macOS 10.0+

``` source
func forKey(_ key: String) -> NSScriptClassDescription?
```

## Parameters 

`key`  

The identifying key for an attribute or relationship of the receiver.

## Return Value

The instance of `NSScriptClassDescription` for the type of the attribute or relationship specified by `key`. Returns `nil` if no scriptable property corresponds to `key`.

## See Also

### Getting a Script Class Description

init?(for: AnyClass)

Returns the class description for the specified class or, if it is not scriptable, for the first superclass that is.

var superclass: NSScriptClassDescription?

Returns the class description instance for the superclass of the receiver’s class.

