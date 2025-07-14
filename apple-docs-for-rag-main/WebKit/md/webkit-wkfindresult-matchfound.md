

- WebKit
- WKFindResult
-  matchFound 

Instance Property

# matchFound

A Boolean value that indicates whether the web view found a match during the search.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@MainActor
var matchFound: Bool { get }
```

## Discussion

The value of this property is true if the web view found a match, or false if it didn’t.

