

- WatchKit
- WKExtensionDelegate
-  userDidAcceptCloudKitShare(with:) 

Instance Method

# userDidAcceptCloudKitShare(with:)

Tells the delegate that the app has access to shared information in CloudKit.

watchOS 7.0+

``` source
@MainActor
optional func userDidAcceptCloudKitShare(with cloudKitShareMetadata: CKShareMetadata)
```

## Parameters 

`cloudKitShareMetadata`  

Information about the CloudKit data that is available to the app. Use this object to retrieve information about the CKShare object and the associated records that are available.

## Discussion

Use this method to respond to a CloudKit Sharing invitation. In your implementation, accept the share by scheduling a CKAcceptSharesOperation object that contains the provided metadata object. After the user accepts the share, you can begin fetching records and incorporating the resulting data into your app.

The system launches the app, as necessary, before calling this method.

