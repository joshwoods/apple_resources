

- Core Spotlight
- CSUserQueryContext
-  maxRankedResultCount 

Instance Property

# maxRankedResultCount

The maximum number of ranked results to return during the query.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var maxRankedResultCount: Int { get set }
```

## Discussion

Spotlight ranks a limited number of results by default, but you can change the default value to improve performance or better suit your app’s interface. For example, you might want to return only the five most relevant results due to space constraints in your UI.

## See Also

### Configuring the ranked results behavior

var enableRankedResults: Bool

A Boolean value that indicates whether the query sorts results by their relevance.

