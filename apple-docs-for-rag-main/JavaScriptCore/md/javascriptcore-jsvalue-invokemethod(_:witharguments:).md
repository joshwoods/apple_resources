

- JavaScriptCore
- JSValue
-  invokeMethod(\_:withArguments:) 

Instance Method

# invokeMethod(\_:withArguments:)

Calls the named JavaScript method on the value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func invokeMethod(
    _ method: String!,
    withArguments arguments: [Any]!
) -> JSValue!
```

## Parameters 

`method`  

The name of a method on the value; that is, of a field whose contents are a function value.

`arguments`  

The parameters to pass to the method. The objects in this array must be other JSValue objects or objects that can be converted to JavaScript values using the methods listed in the Creating JavaScript Values section in JSValue.

## Return Value

The result of calling the value as a constructor, or `nil` if the value cannot be treated as a JavaScript constructor.

## Discussion

Calling this Objective-C method first uses the forProperty(_:) method to look up the named field of the JavaScript value. Then, JavaScriptCore treats that field’s contents as a JavaScript function and sets the JavaScript `this` keyword to refer to this JSValue instance.

## See Also

### Working with Function and Constructor Values

func call(withArguments: [Any]!) -> JSValue!

Invokes the value as a JavaScript function.

func construct(withArguments: [Any]!) -> JSValue!

Invokes the value as a JavaScript constructor.

