

- Local Authentication
- LAContext
-  evaluateAccessControl(\_:operation:localizedReason:reply:) 

Instance Method

# evaluateAccessControl(\_:operation:localizedReason:reply:)

Evaluates an access control for a given operation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 3.0+

``` source
func evaluateAccessControl(
    _ accessControl: SecAccessControl,
    operation: LAAccessControlOperation,
    localizedReason: String,
    reply: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func evaluateAccessControl(
    _ accessControl: SecAccessControl,
    operation: LAAccessControlOperation,
    localizedReason: String
) async throws -> Bool
```

## Parameters 

`accessControl`  

The access control to be evaluated.

`operation`  

The operation for the access control to be evaluated. For possible values, see LAAccessControlOperation.

`localizedReason`  

The app-provided reason for requesting authentication, which displays in the authentication dialog presented to the user.

`reply`  

A block that is executed when access control evaluation finishes. This block is evaluated on a private queue internal to the framework in an unspecified threading context.

success  
`true` if policy evaluation succeeded, otherwise `false`.

error  
`nil` if policy evaluation succeeded, an error object that should be presented to the user otherwise. See LAError.Code for possible error codes

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func evaluateAccessControl(_ accessControl: SecAccessControl, operation: LAAccessControlOperation, localizedReason: String) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method asynchronously evaluates an access control. Evaluating an access control may involve prompting the user for various kinds of interaction or authentication. The actual behavior is dependent on the access control and device type. It can also be affected by installed configuration profiles.

The localized string you present to the user should provide a clear reason for why you are requesting they authenticate themselves, and what action you will be taking based on that authentication. This string should be provided in the user’s current language and should be short and clear. It should not contain the app name, because that appears elsewhere in the authentication dialog. In macOS this appears in the dialog title, and in iOS this appears in the dialog subtitle.

You should not assume that a previous successful evaluation of an access control necessarily leads to a subsequent successful evaluation. Access control evaluation can fail for various reasons, including cancelation by the user or the system.

## See Also

### Evaluating access controls

enum LAAccessControlOperation

Operations to be evaluated for access control.

var interactionNotAllowed: Bool

A Boolean value indicating whether authentication can be interactive.

