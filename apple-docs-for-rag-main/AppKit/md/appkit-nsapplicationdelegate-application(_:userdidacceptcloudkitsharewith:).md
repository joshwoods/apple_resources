

- AppKit
- NSApplicationDelegate
-  application(\_:userDidAcceptCloudKitShareWith:) 

Instance Method

# application(\_:userDidAcceptCloudKitShareWith:)

Tells the delegate when the user accepts a CloudKit sharing invitation.

macOS 10.12+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    userDidAcceptCloudKitShareWith metadata: CKShareMetadata
)
```

## Parameters 

`application`  

The shared app object.

`metadata`  

The metadata associated with the invitation. Use the URL of the metadata’s CKShare object and the containerIdentifier property to schedule a CKAcceptSharesOperation object.

## Discussion

Use the provided metadata to begin sharing the specified content with the current user. For more information, see CloudKit.

