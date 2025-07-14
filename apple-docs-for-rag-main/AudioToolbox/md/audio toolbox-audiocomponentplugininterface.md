

- Audio Toolbox
-  AudioComponentPlugInInterface 

Structure

# AudioComponentPlugInInterface

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioComponentPlugInInterface
```

## Topics

### Initializers

init(Open: (UnsafeMutableRawPointer, AudioComponentInstance) -> OSStatus, Close: (UnsafeMutableRawPointer) -> OSStatus, Lookup: (Int16) -> AudioComponentMethod?, reserved: UnsafeMutableRawPointer?)

init(Open: (UnsafeMutableRawPointer, AudioComponentInstance) -> OSStatus, Close: (UnsafeMutableRawPointer) -> OSStatus, Lookup: (Int16) -> AudioComponentMethod?, reserved: UnsafeMutableRawPointer?)

### Instance Properties

var Close: (UnsafeMutableRawPointer) -> OSStatus

var Lookup: (Int16) -> AudioComponentMethod?

var Open: (UnsafeMutableRawPointer, AudioComponentInstance) -> OSStatus

var reserved: UnsafeMutableRawPointer?

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Getting Information About a Component

func AudioComponentInstanceCanDo(AudioComponentInstance, Int16) -> Bool

Determines if an audio component instance implements a particular function.

func AudioComponentGetDescription(AudioComponent, UnsafeMutablePointer&lt;AudioComponentDescription>) -> OSStatus

Gets the class description, as an `AudioComponentDescription` structure, of an audio component.

func AudioComponentCopyName(AudioComponent, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Returns the generic name of an audio component.

func AudioComponentGetVersion(AudioComponent, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the version of an audio component in hexadecimal form as `0xMMMMmmDD` (major, minor, dot).

func AudioComponentCopyIcon(AudioComponent) -> UIImage?

func AudioComponentCopyConfigurationInfo(AudioComponent, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

typealias AudioComponentMethod

