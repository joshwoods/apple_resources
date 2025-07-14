

- ShazamKit
- SHManagedSession
-  results 

Instance Property

# results

The results as an asynchronous sequence of matches.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final var results: SHSession.Results { get }
```

## Discussion

This session continues to return results until the sequence is exhausted or the app calls cancel().

## See Also

### Returning queries

func result() async -> SHSession.Result

Performs an asynchronous match with a single signature.

func cancel()

Cancels the currently running match attempt.

func prepare() async

Preallocates the resources needed for a match, which increases the responsiveness of matches.

