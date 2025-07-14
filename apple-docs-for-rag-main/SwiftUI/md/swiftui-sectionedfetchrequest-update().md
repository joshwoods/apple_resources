

- SwiftUI
- SectionedFetchRequest
-  update() 

Instance Method

# update()

Updates the fetched results.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
func update()
```

Available when `SectionIdentifier` conforms to `Hashable` and `Result` conforms to `NSFetchRequestResult`.

## Discussion

SwiftUI calls this function before rendering a view’s body to ensure the view has the most recent fetched results.

## See Also

### Getting the fetched results

var wrappedValue: SectionedFetchResults&lt;SectionIdentifier, Result>

The fetched results of the fetch request.

