

- Objective-C Runtime
- NSObject
-  webScriptName(forKey:) 

Type Method

# webScriptName(forKey:)

Returns the scripting environment name for an attribute specified by a key.

macOS 10.4+

``` source
class func webScriptName(forKey name: UnsafePointer!) -> String!
```

## Parameters 

`name`  

The name of the attribute.

## Return Value

The name used to represent the attribute in the scripting environment.

## See Also

### Getting attributes

class func webScriptName(for: Selector!) -> String!

Returns the scripting environment name for a selector.

class func isSelectorExcluded(fromWebScript: Selector!) -> Bool

Returns whether a selector should be hidden from the scripting environment.

class func isKeyExcluded(fromWebScript: UnsafePointer&lt;CChar>!) -> Bool

Returns whether a key should be hidden from the scripting environment.

