

- Objective-C Runtime
- NSObject
-  isKeyExcluded(fromWebScript:) 

Type Method

# isKeyExcluded(fromWebScript:)

Returns whether a key should be hidden from the scripting environment.

macOS 10.4+

``` source
class func isKeyExcluded(fromWebScript name: UnsafePointer!) -> Bool
```

## Parameters 

`name`  

The name of the attribute.

## Return Value

YES if the attribute specified by `name` should be hidden from the scripting environment; otherwise, NO.

## Discussion

The default value is YES.

## See Also

### Getting attributes

class func webScriptName(forKey: UnsafePointer&lt;CChar>!) -> String!

Returns the scripting environment name for an attribute specified by a key.

class func webScriptName(for: Selector!) -> String!

Returns the scripting environment name for a selector.

class func isSelectorExcluded(fromWebScript: Selector!) -> Bool

Returns whether a selector should be hidden from the scripting environment.

