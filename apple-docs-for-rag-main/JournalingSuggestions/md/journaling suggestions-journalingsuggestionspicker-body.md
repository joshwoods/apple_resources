

- Journaling Suggestions
- JournalingSuggestionsPicker
-  body 

Instance Property

# body

The content and behavior of the view.

iOS 17.2+

``` source
@MainActor @preconcurrency
var body: some View { get }
```

## Discussion

When you implement a custom view, you must implement a computed body property to provide the content for your view. Return a view that’s composed of built-in views that SwiftUI provides, plus other composite views that you’ve already defined:

```
```

For more information about composing views and a view hierarchy, see Declaring a custom view.

