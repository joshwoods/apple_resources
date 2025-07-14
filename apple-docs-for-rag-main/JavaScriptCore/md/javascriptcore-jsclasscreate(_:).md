

- JavaScriptCore
-  JSClassCreate(\_:) 

Function

# JSClassCreate(\_:)

Creates a JavaScript class.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSClassCreate(_ definition: UnsafePointer!) -> JSClassRef!
```

## Parameters 

`definition`  

A JSClassDefinition that defines the class.

## Return Value

A JSClassRef with the specified definition suitable for use with JSObjectMake(_:_:_:). Ownership follows The Create Rule.

## See Also

### Working with Classes

func JSClassRelease(JSClassRef!)

Releases a JavaScript class.

func JSClassRetain(JSClassRef!) -> JSClassRef!

Retains a JavaScript class.

let kJSClassDefinitionEmpty: JSClassDefinition

A class definition structure of the current version that contains null pointers and has no attributes.

struct JSClassDefinition

A structure that contains properties and callbacks that define a type of object.

JSClassAttribute

A JavaScript class attribute.

