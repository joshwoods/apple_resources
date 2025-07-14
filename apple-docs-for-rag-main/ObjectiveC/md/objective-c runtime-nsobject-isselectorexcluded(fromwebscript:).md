

- Objective-C Runtime
- NSObject
-  isSelectorExcluded(fromWebScript:) 

Type Method

# isSelectorExcluded(fromWebScript:)

Returns whether a selector should be hidden from the scripting environment.

macOS 10.4+

``` source
class func isSelectorExcluded(fromWebScript selector: Selector!) -> Bool
```

## Parameters 

`selector`  

The selector.

## Return Value

YES if the selector specified by `aSelector` should be hidden from the scripting environment; otherwise, NO.

## Discussion

Only methods with valid parameters and return types are exported to the WebKit JavaScript environment. The valid types are Objective-C objects and scalars. The default value is YES.

## See Also

### Getting attributes

class func webScriptName(forKey: UnsafePointer&lt;CChar>!) -> String!

Returns the scripting environment name for an attribute specified by a key.

class func webScriptName(for: Selector!) -> String!

Returns the scripting environment name for a selector.

class func isKeyExcluded(fromWebScript: UnsafePointer&lt;CChar>!) -> Bool

Returns whether a key should be hidden from the scripting environment.

