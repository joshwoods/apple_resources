

- AppKit
- NSSuggestionItemResponse
-  phase 

Instance Property

# phase

Describes the phase of results. In other words, whether this batch of items represents an intermediate set of results–and more are coming, or whether these results are complete/final. Defaults to `.final`.

macOS 15.0+

``` source
var phase: NSSuggestionItemResponse.Phase
```

## Discussion

Note

This controls whether or not a indeterminate spinner appears by the control and suggestions menu to indicate to the user that there may be any/more/different/updated suggestions coming.

Note

Once a final set of results have been provided, the control will ignore subsequent provisions until the search request changes.

