

- UIKit
- UIDocument
-  userInteractionNoLongerPermitted(forError:) 

Instance Method

# userInteractionNoLongerPermitted(forError:)

Indicates when it’s no longer safe to proceed without immediately handling the error.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func userInteractionNoLongerPermitted(forError error: any Error)
```

## Parameters 

`error`  

An error object encapsulating information about the error.

## Discussion

UIKit calls this method when it’s no longer safe to proceed without immediately handling the error, such as when the application is being suspended. Subclasses that override this method must immediately end error handling (including dismissing any interactive user interface) and call finishedHandlingError(_:recovered:) before returning. It’s only necessary to override this method if you override handleError(_:userInteractionPermitted:) without invoking the superclass implementation (`super`).

## See Also

### Resolving conflicts and handling errors

func handleError(any Error, userInteractionPermitted: Bool)

Handles an error that occurs during an attempt to read, save, or revert a document.

func finishedHandlingError(any Error, recovered: Bool)

Tells UIKit that you finished handling the error.

