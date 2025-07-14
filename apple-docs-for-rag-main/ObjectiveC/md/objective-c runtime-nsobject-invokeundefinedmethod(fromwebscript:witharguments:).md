

- Objective-C Runtime
- NSObject
-  invokeUndefinedMethod(fromWebScript:withArguments:) 

Instance Method

# invokeUndefinedMethod(fromWebScript:withArguments:)

Handles undefined method invocation from the scripting environment.

macOS 10.4+

``` source
func invokeUndefinedMethod(
    fromWebScript name: String!,
    withArguments arguments: [Any]!
) -> Any!
```

## Parameters 

`name`  

The name of the undefined method.

`arguments`  

The arguments passed to the undefined method.

## Return Value

The result of invoking the undefined method.

## Discussion

This method is invoked when a script attempts to invoke a method not directly exported to the scripting environment. You should return the result of the invocation, converted appropriately for the scripting environment.

## See Also

### Invoking methods

func invokeDefaultMethod(withArguments: [Any]!) -> Any!

Executes when a script attempts to invoke a method on an exposed object directly.

