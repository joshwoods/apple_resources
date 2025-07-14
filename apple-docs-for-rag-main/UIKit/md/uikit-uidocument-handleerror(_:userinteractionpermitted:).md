

- UIKit
- UIDocument
-  handleError(\_:userInteractionPermitted:) 

Instance Method

# handleError(\_:userInteractionPermitted:)

Handles an error that occurs during an attempt to read, save, or revert a document.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func handleError(
    _ error: any Error,
    userInteractionPermitted: Bool
)
```

## Parameters 

`error`  

An object encapsulating information about an error encountered in an attempt to open, save, or revert a document. The error domain is NSCocoaErrorDomain. The error code is one of the `enum` constants declared in `FoundationErrors.h`.

`userInteractionPermitted`  

If false, no attempt is (or should be) made to present a modal view to the user. This value can be false in cases such as when a save operation fails while the application is being suspended. If this parameter is true, UIKit or your override may present error information to the user in a modal view and (optionally) allow the user to resolve the error.

## Discussion

Typical UIDocument subclasses don’t need to call or override this method. Instead, they can observe the stateChangedNotification notification to be notified of changes in document state. In their notification handler, they can check the value of the documentState property and proceed accordingly. See Resolve conflicts and handle errors for a discussion of this.

If you’re using managed documents (instances of the UIManagedDocument subclass), you must subclass this method and, if desired, the finishedHandlingError(_:recovered:) method. Subclassing allows your app to observe errors in saving or validation. The stateChangedNotification notification doesn’t contain a `userInfo` dictionary and so doesn’t convey specific error information.

If you directly call any of the advanced reading and writing methods that have an error-object parameter (for example, writeContents(_:andAttributes:safelyTo:for:)) and that call returns an NSError object by indirection, you should call this method (handleError(_:userInteractionPermitted:)), passing in the error object.

This method is called by the default implementations of open(completionHandler:) and save(to:for:completionHandler:) when UIDocument encounters a reading or writing error, respectively.

If you override this method and don’t invoke the superclass implementation (`super`), you’re responsible for the following:

- Calling finishedHandlingError(_:recovered:) when you’re finished handling the error — for example, when the application doesn’t require any additional user feedback about the error.

- Implementing userInteractionNoLongerPermitted(forError:) to conclude error handling immediately. If `userInteractionPermitted` is false, you should immediately handle the error and call finishedHandlingError(_:recovered:) within the context of the handleError(_:userInteractionPermitted:).

## See Also

### Resolving conflicts and handling errors

func finishedHandlingError(any Error, recovered: Bool)

Tells UIKit that you finished handling the error.

func userInteractionNoLongerPermitted(forError: any Error)

Indicates when it’s no longer safe to proceed without immediately handling the error.

