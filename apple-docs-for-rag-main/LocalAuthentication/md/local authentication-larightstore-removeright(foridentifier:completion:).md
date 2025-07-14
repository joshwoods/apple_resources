

- Local Authentication
- LARightStore
-  removeRight(forIdentifier:completion:) 

Instance Method

# removeRight(forIdentifier:completion:)

Removes a right from the right store given its unique identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func removeRight(
    forIdentifier identifier: String,
    completion handler: @escaping ((any Error)?) -> Void
)
```

``` source
func removeRight(forIdentifier identifier: String) async throws
```

## Parameters 

`identifier`  

The identifier for the right to remove.

`handler`  

A completion handler to call when the removal operation completes.

`error`  
An error object that indicates why the removal operation failed, or `nil` if it succeeded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func removeRight(forIdentifier identifier: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Removing a right also removes any resources stored along with the right, such as secrets.

## See Also

### Removing stored rights

func removeRight(LAPersistedRight, completion: ((any Error)?) -> Void)

Removes a right from the right store given an instance of that right.

func removeAllRights(completion: ((any Error)?) -> Void)

Removes all rights associated with this client from the right store.

