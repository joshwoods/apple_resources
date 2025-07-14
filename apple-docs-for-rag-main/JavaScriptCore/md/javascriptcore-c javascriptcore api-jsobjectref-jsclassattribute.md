

- JavaScriptCore
- C JavaScriptCore API
- JSObjectRef
-  JSClassAttribute 

API Collection

# JSClassAttribute

A JavaScript class attribute.

## Topics

### Constants

var kJSClassAttributeNone: Int

An attribute that specifies that a class has no special attributes.

var kJSClassAttributeNoAutomaticPrototype: Int

An attribute that specifies that a class doesn’t automatically generate a shared prototype for its instance objects.

## See Also

### Working with Classes

func JSClassCreate(UnsafePointer&lt;JSClassDefinition>!) -> JSClassRef!

Creates a JavaScript class.

func JSClassRelease(JSClassRef!)

Releases a JavaScript class.

func JSClassRetain(JSClassRef!) -> JSClassRef!

Retains a JavaScript class.

let kJSClassDefinitionEmpty: JSClassDefinition

A class definition structure of the current version that contains null pointers and has no attributes.

struct JSClassDefinition

A structure that contains properties and callbacks that define a type of object.

