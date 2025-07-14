

- SwiftUI
- DropInfo
-  itemProviders(for:) 

Instance Method

# itemProviders(for:)

Finds item providers that conform to at least one of the specified uniform type identifiers.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func itemProviders(for contentTypes: [UTType]) -> [NSItemProvider]
```

Show all declarations

## Parameters 

`contentTypes`  

The uniform type identifiers to query for.

## Return Value

The item providers that conforms to `contentTypes`.

## Discussion

This function is only valid during the `performDrop()` action.

