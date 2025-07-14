

- Translation
- TranslationSession
- TranslationSession.Configuration
-  invalidate() 

Instance Method

# invalidate()

Invalidate the current translation session to re-run it again with new content.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
mutating func invalidate()
```

## Discussion

Call this method when you want to translate new content using the same source and target languages. When you do, it causes the `View/translationTask(_:action:)` function to call its `action` closure and translate the content again.

