

- CoreAudioKit
-  AUGenericView 

Class

# AUGenericView

A view that provides a generic user interface for a Cocoa audio unit.

macOS 10.4+

``` source
@MainActor
class AUGenericView
```

## Topics

### Creating a Generic View

init(audioUnit: AudioUnit)

Creates a generic view for an audio unit, setting all display flags.

init(audioUnit: AudioUnit, displayFlags: AUGenericViewDisplayFlags)

Initializes a generic view for an audio unit, setting specific display flags.

### Configuring a View

var showsExpertParameters: Bool

Indicates whether or not controls for expert audio unit parameters are displayed in the generic view.

### Accessing the Audio Unit

var audioUnit: AudioUnit

The audio unit associated with the generic view.

## Relationships

### Inherits From

- NSView

### Conforms To

- AUCustomViewPersistentData
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

## See Also

### Audio Units

class AUViewController

The base class to extend when creating a custom user interface for an audio unit.

class AUAudioUnitViewConfiguration

A configuration object that describes how to present the audio unit’s user interface.

class AUPannerView

A view that provides a specialized user interface for a Cocoa-based panner audio unit.

protocol AUCustomViewPersistentData

A protocol that defines the methods an Audio Unit host calls to manage view data.

