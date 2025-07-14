

- ClockKit
- CLKWatchFaceLibrary
-  addWatchFace(at:completionHandler:) 

Instance Method

# addWatchFace(at:completionHandler:)

Adds a watch face from the app’s bundle.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.0+

``` source
func addWatchFace(
    at fileURL: URL,
    completionHandler handler: @escaping ((any Error)?) -> Void
)
```

``` source
func addWatchFace(at fileURL: URL) async throws
```

## Parameters 

`fileURL`  

A file URL for a watch face file.

`handler`  

A block that ClockKit calls after adding the watch face. The block takes the following parameter:

error  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Mentioned in 

Sharing an Apple Watch face

## Discussion

Call this method to load a watch face file. The URL must point to a *watch file*, a watch face that your app has downloaded, or a watch face stored in your app bundle. All of the complications on the watch face must come from apps that have a valid App Store ID, such as an app from the App Store or a TestFlight build. If you try to use complications from a development build, the system won’t recognize the development ID as a valid App Store ID.

In iOS, use the WCSession class’s isPaired method to verify that the user has a paired Apple Watch before presenting UI to share the watch face.

Note

Some newer watch faces are not available on Apple Watch Series 3. Additionally, users can only add Nike and Hermès watch faces to the respective hardware. If you share a watch face that isn’t available on all watches running watchOS 7, check for errors when calling addWatchFace(at:completionHandler:), and provide a fallback face that can be installed on all watches running watchOS 7 or later. For a list of watch faces supported on Apple Watch Series 3, see Apple Watch faces and their features.

If you call this method on a device that doesn’t support the Watch app or watch faces, this method reports an error.

