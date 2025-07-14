

- ShazamKit
- SHManagedSession
-  prepare() 

Instance Method

# prepare()

Preallocates the resources needed for a match, which increases the responsiveness of matches.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final func prepare() async
```

## See Also

### Returning queries

func result() async -> SHSession.Result

Performs an asynchronous match with a single signature.

var results: SHSession.Results

The results as an asynchronous sequence of matches.

func cancel()

Cancels the currently running match attempt.

