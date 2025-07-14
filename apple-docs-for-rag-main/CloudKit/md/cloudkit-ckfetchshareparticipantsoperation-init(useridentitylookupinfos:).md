

- CloudKit
- CKFetchShareParticipantsOperation
-  init(userIdentityLookupInfos:) 

Initializer

# init(userIdentityLookupInfos:)

Creates an operation for generating share participants from the specified user data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(userIdentityLookupInfos: [CKUserIdentity.LookupInfo])
```

## Parameters 

`userIdentityLookupInfos`  

The user data for the participants. If you specify `nil`, you must assign a value to the userIdentityLookupInfos property before you execute this operation.

## Discussion

After you create the operation, assign a handler to the fetchShareParticipantsCompletionBlock property to process the results.

## See Also

### Creating an Operation

init()

Creates an empty operation.

