

- UIKit
- UISearchToken
-  representedObject 

Instance Property

# representedObject

The object represented by the search token.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var representedObject: Any? { get set }
```

## Discussion

Use this property to keep information required to restore a search from state restoration, paste a search token, or perform the user’s search.

## See Also

### Creating a search token

init(icon: UIImage?, text: String)

Creates a search token with the specified text and icon (if any).

