

- ARKit
- ARHitTestResult
-  type Deprecated

Instance Property

# type

The kind of detected feature the search result represents.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
var type: ARHitTestResult.ResultType { get }
```

Deprecated

Use raycasting

## Discussion

You specify one or more result types to search for when calling a hit-testing method. A result object has only one result type.

## See Also

### Identifying Results

struct ResultType

Possible types for specifying a hit-test search, or for the result of a hit-test search.

Deprecated

var anchor: ARAnchor?

The anchor representing the detected surface, if any.

Deprecated

