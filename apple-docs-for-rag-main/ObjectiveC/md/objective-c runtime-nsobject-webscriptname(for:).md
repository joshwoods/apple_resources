

- Objective-C Runtime
- NSObject
-  webScriptName(for:) 

Type Method

# webScriptName(for:)

Returns the scripting environment name for a selector.

macOS 10.4+

``` source
class func webScriptName(for selector: Selector!) -> String!
```

## Parameters 

`selector`  

The selector.

## Return Value

The name used to represent the selector in the scripting environment.

## Discussion

It is your responsibility to ensure that the returned name is unique to the script invoking this method. If this method returns `nil` or you do not implement it, the default name for the selector is constructed as follows:

- A colon (”:”) in the Objective-C selector is replaced by an underscore (”\_”).

- An underscore in the Objective-C selector is prefixed with a dollar sign (”\$”).

- A dollar sign in the Objective-C selector is prefixed with another dollar sign.

The following table shows examples of how the default name is constructed:

| Objective-C selector             | Default script name for selector   |
|----------------------------------|------------------------------------|
| `setFlag:`                       | `setFlag_`                         |
| `setFlag:forKey:withAttributes:` | `setFlag_forKey_withAttributes_`   |
| `propertiesForExample_Object:`   | `propertiesForExample$_Object_`    |
| `set_$_forKey:withDictionary:`   | `set$_$$_$_forKey_withDictionary_` |

Since the default construction for a method name can be confusing depending on its Objective-C name, you should implement this method and return a more human-readable name.

## See Also

### Getting attributes

class func webScriptName(forKey: UnsafePointer&lt;CChar>!) -> String!

Returns the scripting environment name for an attribute specified by a key.

class func isSelectorExcluded(fromWebScript: Selector!) -> Bool

Returns whether a selector should be hidden from the scripting environment.

class func isKeyExcluded(fromWebScript: UnsafePointer&lt;CChar>!) -> Bool

Returns whether a key should be hidden from the scripting environment.

