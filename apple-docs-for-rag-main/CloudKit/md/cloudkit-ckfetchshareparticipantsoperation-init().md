

- CloudKit
- CKFetchShareParticipantsOperation
-  init() 

Initializer

# init()

Creates an empty operation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init()
```

## Discussion

You can use this operation only once.

Note

If you don’t set userIdentityLookupInfos prior to executing the operation, it returns immediately with no results.

## See Also

### Creating an Operation

convenience init(userIdentityLookupInfos: [CKUserIdentity.LookupInfo])

Creates an operation for generating share participants from the specified user data.

