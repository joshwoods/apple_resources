

- AppKit
- NSDocument
-  move(to:completionHandler:) 

Instance Method

# move(to:completionHandler:)

Moves the document’s file to the given URL.

macOS 10.8+

``` source
@MainActor
func move(
    to url: URL,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
@MainActor
func move(to url: URL) async throws
```

## Parameters 

`url`  

The location where the file will ultimately end up, if the move is successful.

`completionHandler`  

The completion handler block object passed in to be invoked at some point in the future, perhaps after the method invocation has returned. The completion handler must be invoked on the main thread. On output, a `nil` error is passed if the move is successful; otherwise an NSError object is passed that encapsulates the reason for failure.

## Discussion

The default implementation of this method replaces any file that may currently exist at the given URL with the one being moved, as necessary.

## See Also

### Related Documentation

func moveToUbiquityContainer(Any?)

Moves the document to the user’s iCloud storage.

### Moving the Document

func move(Any?)

Moves the document to a new location in response to the user choosing the Move To… menu item.

func move(completionHandler: ((Bool) -> Void)?)

Moves the document to a user-selected location.

