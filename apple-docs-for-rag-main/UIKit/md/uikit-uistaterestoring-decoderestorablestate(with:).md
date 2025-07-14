

- UIKit
- UIStateRestoring
-  decodeRestorableState(with:) 

Instance Method

# decodeRestorableState(with:)

Decodes and restores state-related information for the object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func decodeRestorableState(with coder: NSCoder)
```

## Parameters 

`coder`  

The coder object to use to decode the state of the view.

## Mentioned in 

About the UI restoration process

## Discussion

If your app supports state restoration, you can implement this method on any object for which you also overrode the encodeRestorableState(with:) method. Your implementation of this method should read any saved state information from the archive and use it to restore the object to its previous configuration. If your encodeRestorableState(with:) method called `super`, this method should similarly call `super` at some point in its implementation.

## See Also

### Encoding and decoding the object

func encodeRestorableState(with: NSCoder)

Encodes state-related information for the object.

func applicationFinishedRestoringState()

Called after all objects have had a chance to decode their state.

