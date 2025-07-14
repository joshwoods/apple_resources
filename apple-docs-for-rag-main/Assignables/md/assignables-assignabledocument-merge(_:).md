

- Assignables
- AssignableDocument
-  merge(\_:) 

Instance Method

# merge(\_:)

Merge another object of this type into this object.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+visionOS

``` source
@discardableResult
mutating func merge(_ other: AssignableDocument) async throws -> Bool
```

## Parameters 

`other`  

The other object to merge into this one.

## Return Value

`true`, if the merge caused a mutation.

