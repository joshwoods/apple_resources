

- Translation
- TranslationSession
- TranslationSession.BatchResponse
- TranslationSession.BatchResponse.AsyncIterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
mutating func next() async throws -> TranslationSession.BatchResponse.Element?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

