

- WebKit
- WebScriptObject
-  evaluateWebScript(\_:) Deprecated

Instance Method

# evaluateWebScript(\_:)

Returns the result of evaluating a script in the scripting environment.

macOS 10.4–10.14Deprecated

``` source
func evaluateWebScript(_ script: String!) -> Any!
```

## Parameters 

`script`  

The script to evaluate.

## Return Value

The scripting object. The format of the script is dependent on the target scripting environment. Returns WebUndefined if an exception is thrown in the JavaScript environment or there is no return value.

## See Also

### Executing scripts

func callWebScriptMethod(String!, withArguments: [Any]!) -> Any!

Returns the result of executing a method in the scripting environment.

Deprecated

