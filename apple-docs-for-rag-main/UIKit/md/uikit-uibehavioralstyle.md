

- UIKit
-  UIBehavioralStyle 

Enumeration

# UIBehavioralStyle

Constants that indicate how a control behaves in apps built with Mac Catalyst.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
enum UIBehavioralStyle
```

## Overview

If you build your app with Mac Catalyst and use the Mac idiom, you can specify the preferred behavior style for a control to change its appearance and behavior. For instance, consider an iPad app that displays a slider with a custom thumb image. By default, the Mac version of the app, built with Mac Catalyst, displays a standard macOS slider when the user interface idiom of the app is UIUserInterfaceIdiom.mac.

To provide a consistent appearance of the slider in the iPad and Mac versions of the app, set the preferredBehavioralStyle of the slider to UIBehavioralStyle.pad. This behavioral style tells the slider to behave as if the user interface idiom is UIUserInterfaceIdiom.pad even though the app uses the Mac idiom.

macOS doesn’t scale the interface of apps that use the Mac idiom, so you may need to update your app to accommodate size differences. For example, a slider with a custom thumb image may need a different image for the Mac app than the one used in the iPad app.

```
let slider = UISlider()
slider.minimumValue = 0
slider.maximumValue = 1
slider.value = 0.5
slider.preferredBehavioralStyle = .pad

if slider.traitCollection.userInterfaceIdiom == .mac {
    slider.setThumbImage(#imageLiteral(resourceName: "customSliderThumbMac")), for: .normal)
} else {
    slider.setThumbImage(#imageLiteral(resourceName: "customSliderThumb")), for: .normal)
}
```

To learn more about the Mac idiom, see Choosing a user interface idiom for your Mac app.

## Topics

### Styles

case automatic

A style the system chooses based on the app’s targeted platform.

case pad

A style that indicates that a control appears and behaves as it does in iPadOS.

case mac

A style that indicates that a control appears and behaves as it does in macOS.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the behavioral style

var behavioralStyle: UIBehavioralStyle

The style that determines how the button behaves.

var preferredBehavioralStyle: UIBehavioralStyle

The preferred behavioral style.

