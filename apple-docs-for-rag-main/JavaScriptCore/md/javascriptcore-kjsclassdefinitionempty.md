

- JavaScriptCore
-  kJSClassDefinitionEmpty 

Global Variable

# kJSClassDefinitionEmpty

A class definition structure of the current version that contains null pointers and has no attributes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
let kJSClassDefinitionEmpty: JSClassDefinition
```

## Discussion

Use this constant as a convenience when creating class definitions. For example, to create a class definition with only a finalize method.

```
JSClassDefinition definition = kJSClassDefinitionEmpty; 
definition.finalize = Finalize;
```

## See Also

### Working with Classes

func JSClassCreate(UnsafePointer&lt;JSClassDefinition>!) -> JSClassRef!

Creates a JavaScript class.

func JSClassRelease(JSClassRef!)

Releases a JavaScript class.

func JSClassRetain(JSClassRef!) -> JSClassRef!

Retains a JavaScript class.

struct JSClassDefinition

A structure that contains properties and callbacks that define a type of object.

JSClassAttribute

A JavaScript class attribute.

