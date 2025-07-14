

- UIKit
- UICloudSharingController
-  share 

Instance Property

# share

A reference to the CloudKit share record used by the CloudKit sharing controller.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var share: CKShare? { get }
```

## Discussion

This property provides a reference to the CKShare record used by UICloudSharingController. The property is `nil` if the controller doesn’t have a share record. This can happen when the controller is initialized with the init(preparationHandler:) method and the preparation handler hasn’t yet been called.

