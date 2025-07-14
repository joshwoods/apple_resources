

- SwiftUI
- FetchRequest
-  update() 

Instance Method

# update()

Updates the fetched results.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
mutating func update()
```

Available when `Result` conforms to `NSFetchRequestResult`.

## Discussion

SwiftUI calls this function before rendering a view’s body to ensure the view has the most recent fetched results.

## See Also

### Getting the fetched results

var wrappedValue: FetchedResults&lt;Result>

The fetched results of the fetch request.

