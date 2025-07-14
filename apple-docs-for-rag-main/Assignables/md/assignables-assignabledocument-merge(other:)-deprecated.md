

- Assignables
- AssignableDocument
-  merge(other:) Deprecated

Instance Method

# merge(other:)

Merge another object of this type into this object.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@discardableResult
mutating func merge(other: AssignableDocument) throws -> Bool
```

Deprecated

Use merge(\_:)

## Parameters 

`other`  

The other object to merge into this one.

## Discussion

An exception is thrown if `other` is not a replica of this document.

