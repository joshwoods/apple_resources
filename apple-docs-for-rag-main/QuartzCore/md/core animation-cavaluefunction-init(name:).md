

- Core Animation
- CAValueFunction
-  init(name:) 

Initializer

# init(name:)

Returns the value function object identified by the name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
convenience init?(name: CAValueFunctionName)
```

## Parameters 

`name`  

The name of the value function.

## Return Value

A new `CAValueFunction` instance with the value function specified by the name.

## Discussion

The possible values for `name` are specified in Rotate Value Functions, Scale Value Functions, and Translate Functions.

