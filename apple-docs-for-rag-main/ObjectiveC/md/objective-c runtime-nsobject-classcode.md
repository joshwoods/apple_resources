

- Objective-C Runtime
- NSObject
-  classCode 

Instance Property

# classCode

The receiver’s Apple event type code, as stored in the `NSScriptClassDescription` object for the object’s class.

Mac CatalystmacOS

``` source
var classCode: FourCharCode { get }
```

## Discussion

This property is used by Cocoa’s scripting support classes.

## See Also

### Scripting

var className: String

A string containing the name of the class.

func copyScriptingValue(Any, forKey: String, withProperties: [String : Any]) -> Any?

Creates and returns one or more scripting objects to be inserted into the specified relationship by copying the passed-in value and setting the properties in the copied object or objects.

func newScriptingObject(of: AnyClass, forValueForKey: String, withContentsValue: Any?, properties: [String : Any]) -> Any?

Creates and returns an instance of a scriptable class, setting its contents and properties, for insertion into the relationship identified by the key.

var scriptingProperties: [String : Any]?

An `NSString`-keyed dictionary of the receiver’s scriptable properties.

func scriptingValue(for: NSScriptObjectSpecifier) -> Any?

Given an object specifier, returns the specified object or objects in the receiving container.

