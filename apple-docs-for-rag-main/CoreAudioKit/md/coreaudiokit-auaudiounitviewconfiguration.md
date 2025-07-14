

- CoreAudioKit
-  AUAudioUnitViewConfiguration 

Class

# AUAudioUnitViewConfiguration

A configuration object that describes how to present the audio unit’s user interface.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
class AUAudioUnitViewConfiguration
```

## Topics

### Creating a Configuration

init(width: CGFloat, height: CGFloat, hostHasController: Bool)

Creates a new configuration object.

### Accessing Settings

var width: CGFloat

The configured width.

var height: CGFloat

The configured height.

var hostHasController: Bool

A Boolean value that indicates whether the host shows its own control surface in this view configuration.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Audio Units

class AUViewController

The base class to extend when creating a custom user interface for an audio unit.

class AUGenericView

A view that provides a generic user interface for a Cocoa audio unit.

class AUPannerView

A view that provides a specialized user interface for a Cocoa-based panner audio unit.

protocol AUCustomViewPersistentData

A protocol that defines the methods an Audio Unit host calls to manage view data.

