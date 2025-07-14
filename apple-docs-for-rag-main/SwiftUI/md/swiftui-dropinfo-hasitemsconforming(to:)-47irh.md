

- SwiftUI
- DropInfo
-  hasItemsConforming(to:) 

Instance Method

# hasItemsConforming(to:)

Indicates whether at least one item conforms to at least one of the specified uniform type identifiers.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func hasItemsConforming(to contentTypes: [UTType]) -> Bool
```

Show all declarations

## Parameters 

`contentTypes`  

The uniform type identifiers to query for.

## Return Value

Whether at least one item conforms to one of `contentTypes`.

## See Also

### Checking for items

func itemProviders(for: [UTType]) -> [NSItemProvider]

Finds item providers that conform to at least one of the specified uniform type identifiers.

