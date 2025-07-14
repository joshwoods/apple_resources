

- SwiftData
- ModelActor
-  subscript(\_:as:) 

Instance Subscript

# subscript(\_:as:)

Returns the model for the specified identifier, downcast to the appropriate class.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
subscript(
    id: PersistentIdentifier,
    as as: T.Type
) -> T? where T : PersistentModel { get }
```

