

- WatchKit
-  WKInterfaceVolumeControl 

Class

# WKInterfaceVolumeControl

An interface element that provides control of the audio volume from the watch or a paired iPhone.

watchOS 5.0+

``` source
class WKInterfaceVolumeControl
```

## Overview

Configure your app’s audio source and the appearance of the volume control in your storyboard file. Use the WKInterfaceVolumeControl instance to change the volume’s tint color at runtime.

Do not subclass or create instances of this class yourself. Instead, define outlets in your interface controller class and connect them to the corresponding objects in your storyboard file. For example, to refer to a volume control in your interface, define a property with the following syntax in your interface controller class:

- Swift
- Objective-C

```
@IBOutlet weak var myVolumeControl: WKInterfaceVolumeControl!
```

```
@property (weak, nonatomic) IBOutlet WKInterfaceVolumeControl* myVolumeControl;
```

During the initialization of your interface controller, WatchKit creates a new instance of this class and assigns it to your outlet. At that point, you can use the object in your outlet to make changes to the onscreen control.

After selecting the volume control, the user can increase or decrease the audio’s volume using the crown. The system automatically handles changing the audio source’s volume. You cannot access or change the volume programmatically in your app.

### Interface Builder Configuration Options

Xcode lets you configure your volume control in your storyboard file. The following table lists the attributes you can configure and their meaning.

| Attribute | Description |
|----|----|
| Controls Local Volume | The volume control’s audio source. If checked, the control affects the volume of long-form audio playing on the watch. If unchecked, it affects the volume of audio playing on the paired iPhone.  You must set this value at design time. You cannot change its value programmatically. |
| Tint Color | The tint color for the volume control. By default, the system uses the application’s tint color.  The system only applies the tint color to the control’s default state (when the crown is not being used to adjust the volume).  You can change this value programmatically using the setTintColor(_:) method. |

## Topics

### Setting the Tint Color

func setTintColor(UIColor?)

Sets the volume control’s tint color.

### Managing Input from the Digital Crown

func focus()

Sets the volume control as the focus for input from the Digital Crown.

func resignFocus()

Removes focus from the volume control, causing it to stop receiving input from the Digital Crown.

### SwiftUI

init(origin: WKInterfaceVolumeControl.Origin)

Creates a volume control for use in SwiftUI.

enum Origin

The source of the audio managed by the volume control.

## Relationships

### Inherits From

- WKInterfaceObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio

Playing Background Audio

Enable background audio in your app to provide a seamless playback experience.

Adding a Now Playing View

Provide a view that controls the currently playing audio from your app.

PUICAutoLaunchAudioOptOut

A Boolean value that indicates whether a watchOS app should opt out of automatically launching when its companion iOS app starts playing audio content.

class WKAudioFilePlayer

An object that controls playback of a single audio item.

Deprecated

class WKAudioFileQueuePlayer

An object that controls playback of one or more audio items.

Deprecated

class WKAudioFilePlayerItem

An object that manages the presentation state of an audio file while it is playing.

Deprecated

class WKAudioFileAsset

An object that stores a reference to an audio file and provides metadata information about that file.

Deprecated

