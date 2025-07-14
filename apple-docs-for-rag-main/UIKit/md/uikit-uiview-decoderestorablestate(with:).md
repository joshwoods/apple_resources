

- UIKit
- UIView
-  decodeRestorableState(with:) 

Instance Method

# decodeRestorableState(with:)

Decodes and restores state-related information for the view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func decodeRestorableState(with coder: NSCoder)
```

## Parameters 

`coder`  

The coder object to use to decode the state of the view.

## Discussion

If your app supports state restoration, you should override this method for any views for which you also overrode the encodeRestorableState(with:) method. Your implementation of this method should use any saved state information to restore the view to its previous configuration. If your encodeRestorableState(with:) method called `super`, this method should similarly call `super` at some point in its implementation.

## See Also

### Preserving and restoring state

var restorationIdentifier: String?

The identifier that determines whether the view supports state restoration.

func encodeRestorableState(with: NSCoder)

Encodes state-related information for the view.

