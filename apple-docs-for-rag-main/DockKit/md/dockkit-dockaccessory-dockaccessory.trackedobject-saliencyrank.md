

- DockKit
- DockAccessory
- DockAccessory.TrackedObject
-  saliencyRank 

Instance Property

# saliencyRank

The saliency rank of the object the dock is tracking. A lower rank indicates higher importance of the object. This property is `nil` if the saliency ranking isn’t set or the object isn’t salient.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var saliencyRank: Int?
```

