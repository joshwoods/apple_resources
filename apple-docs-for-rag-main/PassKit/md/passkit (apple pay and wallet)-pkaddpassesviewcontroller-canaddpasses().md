

- PassKit (Apple Pay and Wallet)
- PKAddPassesViewController
-  canAddPasses() 

Type Method

# canAddPasses()

Returns a Boolean value that indicates whether the device supports adding passes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func canAddPasses() -> Bool
```

## Return Value

true if the device supports adding passes; otherwise, false.

## See Also

### Related Documentation

Wallet Developer Guide

class func isPassLibraryAvailable() -> Bool

Returns a Boolean value that indicates whether the pass library is available.

class PKPassLibrary

Provides an interface to the user’s library of passes.

