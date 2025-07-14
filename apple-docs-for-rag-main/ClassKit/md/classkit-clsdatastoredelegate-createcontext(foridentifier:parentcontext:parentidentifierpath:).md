

- ClassKit
- CLSDataStoreDelegate
-  createContext(forIdentifier:parentContext:parentIdentifierPath:) 

Instance Method

# createContext(forIdentifier:parentContext:parentIdentifierPath:)

Asks the delegate for a new context with the given identifier for the given parent context.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func createContext(
    forIdentifier identifier: String,
    parentContext: CLSContext,
    parentIdentifierPath: [String]
) -> CLSContext?
```

**Required**

## Parameters 

`identifier`  

The identifier of the new context.

`parentContext`  

The parent of the new context.

## Return Value

The new context.

## Discussion

The framework automatically adds the returned context as a child of the parent context and saves the changes. You only need to create, initialize, and return the new context.

