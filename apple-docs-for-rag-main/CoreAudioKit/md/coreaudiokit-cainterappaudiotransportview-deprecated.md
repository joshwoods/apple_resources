

- CoreAudioKit
-  CAInterAppAudioTransportView Deprecated

Class

# CAInterAppAudioTransportView

A view that provides an audio transport user interface.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class CAInterAppAudioTransportView
```

Deprecated

This symbol is no longer recommended. Inter-App Audio is deprecated in iOS 13 and is unavailable when running iPad apps in macOS.

## Topics

### Configuring the View

var isConnected: Bool

var currentTimeLabelFont: UIFont

var isEnabled: Bool

var labelColor: UIColor

var pauseButtonColor: UIColor

var playButtonColor: UIColor

var isPlaying: Bool

var recordButtonColor: UIColor

var isRecording: Bool

var rewindButtonColor: UIColor

func setOutputAudioUnit(AudioUnit)

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Inter-App Audio

class CAInterAppAudioSwitcherView

A view that provides an audio switcher user interface.

Deprecated

