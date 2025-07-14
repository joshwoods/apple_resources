

- CoreAudioKit
-  CABTMIDICentralViewController 

Class

# CABTMIDICentralViewController

A view controller that displays nearby Bluetooth-based MIDI peripherals.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class CABTMIDICentralViewController
```

## Overview

To let the user search for nearby MIDI peripherals, create a new CABTMIDICentralViewController object and then either present it modally or push it onto a UINavigationController view controller. No other configuration of the object is necessary. Once the user interface is visible, the iOS device finds nearby peripherals and displays them to the user. If the user selects a peripheral, it’s automatically paired with this iOS device. The CABTMIDICentralViewController object manages its own user interface and is dismissed automatically.

Once connected, the peripheral appears as a MIDI device, just like any other connected MIDI device. MIDI commands sent to the peripheral are automatically played. For more information, see Core MIDI.

## Relationships

### Inherits From

- UITableViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIScrollViewDelegate
- UIStateRestoring
- UITableViewDataSource
- UITableViewDelegate
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Bluetooth Devices

class CABTLEMIDIWindowController

A window controller that displays nearby Bluetooth-based MIDI peripherals.

class CABTMIDILocalPeripheralViewController

A view controller that advertises an iOS device as a Bluetooth-based MIDI peripheral.

