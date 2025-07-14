

- Swift
- ExpressibleByBooleanLiteral
-  init(booleanLiteral:) 

Initializer

# init(booleanLiteral:)

Creates an instance initialized to the given Boolean value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(booleanLiteral value: Self.BooleanLiteralType)
```

**Required**

## Parameters 

`value`  

The value of the new instance.

## Discussion

Do not call this initializer directly. Instead, initialize a variable or constant using one of the Boolean literals `true` and `false`. For example:

```
let twasBrillig = true
```

In this example, the assignment to the `twasBrillig` constant calls this Boolean literal initializer behind the scenes.

