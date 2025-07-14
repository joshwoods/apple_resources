

- UIKit
- UIDocument
-  finishedHandlingError(\_:recovered:) 

Instance Method

# finishedHandlingError(\_:recovered:)

Tells UIKit that you finished handling the error.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func finishedHandlingError(
    _ error: any Error,
    recovered: Bool
)
```

## Parameters 

`error`  

An error object encapsulating information about the error.

`recovered`  

true if you recovered from the error, otherwise false.

## Discussion

This method is called by default when handling of an error (including any user interaction) is complete. Subclasses need to call this method only if they override handleError(_:userInteractionPermitted:) and do not call the superclass implementation (`super`). If you override this method, you must call `super`.

## See Also

### Resolving conflicts and handling errors

func handleError(any Error, userInteractionPermitted: Bool)

Handles an error that occurs during an attempt to read, save, or revert a document.

func userInteractionNoLongerPermitted(forError: any Error)

Indicates when it’s no longer safe to proceed without immediately handling the error.

