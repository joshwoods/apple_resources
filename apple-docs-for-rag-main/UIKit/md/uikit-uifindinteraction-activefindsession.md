

- UIKit
- UIFindInteraction
-  activeFindSession 

Instance Property

# activeFindSession

The object that manages the state, presentation, and behavior of an active search.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var activeFindSession: UIFindSession? { get }
```

## Discussion

This property returns the session object managing the details of the search. When no seach is active, isFindNavigatorVisible is `false`, this returns `nil`.

## See Also

### Managing the search

func updateResultCount()

Updates the results the interface displays for the active search.

