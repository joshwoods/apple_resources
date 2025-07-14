

- UIKit
- UIStateRestoring
-  encodeRestorableState(with:) 

Instance Method

# encodeRestorableState(with:)

Encodes state-related information for the object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func encodeRestorableState(with coder: NSCoder)
```

## Parameters 

`coder`  

The coder object to use to encode the state of the object.

## Mentioned in 

About the UI preservation process

## Discussion

You can implement this method for any object that has state information you want to preserve. When deciding what data to save, write the smallest amount of data needed to restore the object to its current configuration. The information you save should be data that you could not easily recreate. You can also save references to other objects, such as the view controller that was using the object.

Important

This method is not a substitute for saving your app’s data structures persistently to disk. You should continue to save your app’s actual data to iCloud or the local file system using existing techniques. This method is intended only for saving configuration state or other information related to your app’s user interface. You should consider any data you write to the coder as purgeable and be prepared for it to be unavailable during subsequent launches.

It is strongly recommended that you call `super` at some point during your implementation to give parent classes an opportunity to save information too.

## See Also

### Encoding and decoding the object

func decodeRestorableState(with: NSCoder)

Decodes and restores state-related information for the object.

func applicationFinishedRestoringState()

Called after all objects have had a chance to decode their state.

