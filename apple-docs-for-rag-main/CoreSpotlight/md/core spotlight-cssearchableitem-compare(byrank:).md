

- Core Spotlight
- CSSearchableItem
-  compare(byRank:) 

Instance Method

# compare(byRank:)

Compares two items by rank and returns the result.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func compare(byRank other: CSSearchableItem) -> ComparisonResult
```

## Parameters 

`other`  

The other item to compare against the current one.

## Return Value

A comparison result that indicates the ranked order of the items.

## Discussion

Call this function when you want to compare the current item with the one you specify. The method compares the ranks of the items.

