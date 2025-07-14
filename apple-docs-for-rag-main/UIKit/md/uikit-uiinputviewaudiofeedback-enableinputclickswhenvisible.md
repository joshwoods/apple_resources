

- UIKit
- UIInputViewAudioFeedback
-  enableInputClicksWhenVisible 

Instance Property

# enableInputClicksWhenVisible

Specifies whether or not an input view enables input clicks.

iOSiPadOSMac CatalysttvOS

``` source
@MainActor
optional var enableInputClicksWhenVisible: Bool { get }
```

## Parameters 

`enableInputClicksWhenVisible`  

Return true to enable input clicks by way of the playInputClick() method, or false to disable input clicks. The value is false by default.

## Discussion

In your custom subclass of UIView, implement this property as a getter method. Return true to enable input clicks in your custom input or keyboard accessory view, as follows:

- Swift
- Objective-C

```
var enableInputClicksWhenVisible: Bool {
    return true
}
```

```
- (BOOL) enableInputClicksWhenVisible {
    return YES;
}
```

Input clicks will be produced only if the user has also enabled keyboard clicks in Settings \> Sounds.

