

- Core Text
-  kCTFontManagerRegisteredFontsChangedNotification 

Global Variable

# kCTFontManagerRegisteredFontsChangedNotification

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTFontManagerRegisteredFontsChangedNotification: CFString
```

## Discussion

This is the string to use as the notification name when subscribing to Core Text Font Manager notifications. This notification is posted when fonts are added to the font registry. The client is responsible for registered with the distributed notification center to receive notifications for changes to the session or user scopes, and with a local notification center for changes to the process scope.

## See Also

### Constants

var ATSFONTREF_DEFINED: Int32

var kBSLNIdeographicHighBaseline: Int

let kCTAdaptiveImageProviderAttributeName: CFString

let kCTBackgroundColorAttributeName: CFString

let kCTBaselineClassAttributeName: CFString

let kCTBaselineClassHanging: CFString

let kCTBaselineClassIdeographicCentered: CFString

let kCTBaselineClassIdeographicHigh: CFString

let kCTBaselineClassIdeographicLow: CFString

let kCTBaselineClassMath: CFString

let kCTBaselineClassRoman: CFString

let kCTBaselineInfoAttributeName: CFString

let kCTBaselineOriginalFont: CFString

let kCTBaselineReferenceFont: CFString

let kCTBaselineReferenceInfoAttributeName: CFString

