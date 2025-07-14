

- UIKit
- UIUpdateLink
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that determines whether the UI update link is monitoring UI updates.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

By default, the value of this property is true, which means the system invokes the actions of the UI update link for each UI update.

When the value is false, the UI update link has no effect. Set the value to false if you want to temporarily turn off the UI update link.

