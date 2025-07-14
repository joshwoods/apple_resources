

- CoreAudioKit
-  AUPannerView 

Class

# AUPannerView

A view that provides a specialized user interface for a Cocoa-based panner audio unit.

macOS 10.5+

``` source
@MainActor
class AUPannerView
```

## Topics

### Creating a Panner View

init(audioUnit: AudioUnit)

Creates a panner view for an audio unit.

### Accessing the Audio Unit

var audioUnit: AudioUnit

The panner audio unit associated with the generic panner view.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Audio Units

class AUViewController

The base class to extend when creating a custom user interface for an audio unit.

class AUAudioUnitViewConfiguration

A configuration object that describes how to present the audio unit’s user interface.

class AUGenericView

A view that provides a generic user interface for a Cocoa audio unit.

protocol AUCustomViewPersistentData

A protocol that defines the methods an Audio Unit host calls to manage view data.

