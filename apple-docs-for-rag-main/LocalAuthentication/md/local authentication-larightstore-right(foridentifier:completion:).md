

- Local Authentication
- LARightStore
-  right(forIdentifier:completion:) 

Instance Method

# right(forIdentifier:completion:)

Fetches a previously stored right from the shared right store.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func right(
    forIdentifier identifier: String,
    completion handler: @escaping (LAPersistedRight?, (any Error)?) -> Void
)
```

``` source
func right(forIdentifier identifier: String) async throws -> LAPersistedRight
```

## Parameters 

`identifier`  

The unique identifier of the right.

`handler`  

A completion handler to call when the right access completes.

`right`  
The right that matches the `identifier` you supply.

`error`  
An error object that indicates why the `right` parameter is `nil`, or `nil` if the right parameter is non-`nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func right(forIdentifier identifier: String) async throws -> LAPersistedRight
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Accessing rights

class var shared: LARightStore

A shared object that stores rights.

