

- CoreAudioKit
-  AUCustomViewPersistentData 

Protocol

# AUCustomViewPersistentData

A protocol that defines the methods an Audio Unit host calls to manage view data.

macOS 10.6+

``` source
protocol AUCustomViewPersistentData
```

## Topics

### Accessing View State

var customViewPersistentData: NSDictionary?

Called by the host application to obtain view state data from a custom Cocoa view.

**Required**

## Relationships

### Conforming Types

- AUGenericView

## See Also

### Audio Units

class AUViewController

The base class to extend when creating a custom user interface for an audio unit.

class AUAudioUnitViewConfiguration

A configuration object that describes how to present the audio unit’s user interface.

class AUGenericView

A view that provides a generic user interface for a Cocoa audio unit.

class AUPannerView

A view that provides a specialized user interface for a Cocoa-based panner audio unit.

