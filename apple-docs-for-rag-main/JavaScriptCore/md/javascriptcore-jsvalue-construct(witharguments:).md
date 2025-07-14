

- JavaScriptCore
- JSValue
-  construct(withArguments:) 

Instance Method

# construct(withArguments:)

Invokes the value as a JavaScript constructor.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func construct(withArguments arguments: [Any]!) -> JSValue!
```

## Parameters 

`arguments`  

The parameters to pass to the constructor. The objects in this array must be other JSValue objects or objects that can be converted to JavaScript values using the methods listed in Creating JavaScript Values.

## Return Value

The result of calling the value as a constructor, or `nil` if the value cannot be treated as a JavaScript constructor.

## Discussion

Calling a constructor is equivalent to using the `new` keyword in JavaScript.

## See Also

### Working with Function and Constructor Values

func call(withArguments: [Any]!) -> JSValue!

Invokes the value as a JavaScript function.

func invokeMethod(String!, withArguments: [Any]!) -> JSValue!

Calls the named JavaScript method on the value.

