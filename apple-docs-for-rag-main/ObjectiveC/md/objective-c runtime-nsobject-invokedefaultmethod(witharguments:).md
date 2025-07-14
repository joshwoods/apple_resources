

- Objective-C Runtime
- NSObject
-  invokeDefaultMethod(withArguments:) 

Instance Method

# invokeDefaultMethod(withArguments:)

Executes when a script attempts to invoke a method on an exposed object directly.

macOS 10.4+

``` source
func invokeDefaultMethod(withArguments arguments: [Any]!) -> Any!
```

## Parameters 

`arguments`  

The arguments to be passed to the default method.

## Return Value

The result of invoking the default method.

## See Also

### Invoking methods

func invokeUndefinedMethod(fromWebScript: String!, withArguments: [Any]!) -> Any!

Handles undefined method invocation from the scripting environment.

