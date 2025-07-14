

- Cinematic
- CNScript
-  addUserDecision(\_:) 

Instance Method

# addUserDecision(\_:)

Adds a new user decision, and replaces an existing user decision if the times are identical.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func addUserDecision(_ decision: CNDecision) -> Bool
```

## Parameters 

`decision`  

The decision to add.

## Return Value

A flag indicating whether adding a user decision was successful.

## Discussion

Note

Adding a decision can fail if the decision focuses on a detection or detection group that does not exist or if its time is not within the time range of the Cinematic script.

