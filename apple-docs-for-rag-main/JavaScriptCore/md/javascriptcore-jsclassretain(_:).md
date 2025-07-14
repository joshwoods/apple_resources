

- JavaScriptCore
-  JSClassRetain(\_:) 

Function

# JSClassRetain(\_:)

Retains a JavaScript class.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSClassRetain(_ jsClass: JSClassRef!) -> JSClassRef!
```

## Parameters 

`jsClass`  

The JSClassRef to retain.

## Return Value

A JSClassRef that is the same as `jsClass`.

## See Also

### Working with Classes

func JSClassCreate(UnsafePointer&lt;JSClassDefinition>!) -> JSClassRef!

Creates a JavaScript class.

func JSClassRelease(JSClassRef!)

Releases a JavaScript class.

let kJSClassDefinitionEmpty: JSClassDefinition

A class definition structure of the current version that contains null pointers and has no attributes.

struct JSClassDefinition

A structure that contains properties and callbacks that define a type of object.

JSClassAttribute

A JavaScript class attribute.

