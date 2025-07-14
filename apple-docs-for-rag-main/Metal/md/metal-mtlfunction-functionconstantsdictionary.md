

- Metal
- MTLFunction
-  functionConstantsDictionary 

Instance Property

# functionConstantsDictionary

A dictionary of function constants for a specialized function.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var functionConstantsDictionary: [String : MTLFunctionConstant] { get }
```

**Required**

## Discussion

This property returns a dictionary of the function constants that you need to provide to specialize this function. This property returns an empty dictionary if this function is already specialized or doesn’t declare any function constants.

To create the specialized function, set these constant values in a new MTLFunctionConstantValues object and call the makeFunction(name:constantValues:completionHandler:) method.

