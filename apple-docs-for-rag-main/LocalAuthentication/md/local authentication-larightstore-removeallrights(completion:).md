

- Local Authentication
- LARightStore
-  removeAllRights(completion:) 

Instance Method

# removeAllRights(completion:)

Removes all rights associated with this client from the right store.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func removeAllRights(completion handler: @escaping ((any Error)?) -> Void)
```

``` source
func removeAllRights() async throws
```

## Parameters 

`handler`  

A completion handler to call when the removal operation completes.

`error`  
An error object that indicates why the removal operation failed, or `nil` if it succeeded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func removeAllRights() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Removing rights also removes any resources stored along with the rights, such as secrets.

## See Also

### Removing stored rights

func removeRight(LAPersistedRight, completion: ((any Error)?) -> Void)

Removes a right from the right store given an instance of that right.

func removeRight(forIdentifier: String, completion: ((any Error)?) -> Void)

Removes a right from the right store given its unique identifier.

