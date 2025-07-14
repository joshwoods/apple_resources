

- UIKit
- UIActivityViewController
-  allowsProminentActivity 

Instance Property

# allowsProminentActivity

A Boolean value the system uses to elevate a system activity to make it more prominent.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
@MainActor
var allowsProminentActivity: Bool { get set }
```

## Discussion

The system controls which activities show as prominent in the header of an activity view controller. The default value for this is `true`.

