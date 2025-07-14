

- JavaScriptCore
- JSValue
-  call(withArguments:) 

Instance Method

# call(withArguments:)

Invokes the value as a JavaScript function.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func call(withArguments arguments: [Any]!) -> JSValue!
```

## Parameters 

`arguments`  

The parameters to pass to the function. The objects in this array must be other JSValue objects or objects that can be converted to JavaScript values using the methods listed in the Creating JavaScript Values section in JSValue.

## Return Value

The result of calling the value as a function, or `nil` if the value cannot be treated as a JavaScript function.

## Discussion

In JavaScript, if a function does not explicitly return a value, it implicitly returns the value `undefined`—use the isUndefined property to test for this result.

## See Also

### Working with Function and Constructor Values

func construct(withArguments: [Any]!) -> JSValue!

Invokes the value as a JavaScript constructor.

func invokeMethod(String!, withArguments: [Any]!) -> JSValue!

Calls the named JavaScript method on the value.

