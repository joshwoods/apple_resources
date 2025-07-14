

- App Intents
- IntentCollectionSize
-  init(integerLiteral:) 

Initializer

# init(integerLiteral:)

Creates an instance initialized to the specified integer value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(integerLiteral value: Int)
```

## Parameters 

`value`  

The value to create.

## Discussion

Do not call this initializer directly. Instead, initialize a variable or constant using an integer literal. For example:

```
let x = 23
```

In this example, the assignment to the `x` constant calls this integer literal initializer behind the scenes.

