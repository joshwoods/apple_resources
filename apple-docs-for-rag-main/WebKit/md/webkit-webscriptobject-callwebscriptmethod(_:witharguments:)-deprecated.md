

- WebKit
- WebScriptObject
-  callWebScriptMethod(\_:withArguments:) Deprecated

Instance Method

# callWebScriptMethod(\_:withArguments:)

Returns the result of executing a method in the scripting environment.

macOS 10.4–10.14Deprecated

``` source
func callWebScriptMethod(
    _ name: String!,
    withArguments arguments: [Any]!
) -> Any!
```

## Parameters 

`name`  

The name of the method to invoke.

`arguments`  

The values to pass to the method.

## Return Value

The return value of the method. Returns WebUndefined if an exception is thrown in the JavaScript environment or the method has no return value.

## See Also

### Executing scripts

func evaluateWebScript(String!) -> Any!

Returns the result of evaluating a script in the scripting environment.

Deprecated

