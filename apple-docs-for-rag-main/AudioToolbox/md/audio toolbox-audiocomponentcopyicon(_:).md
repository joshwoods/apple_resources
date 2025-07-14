

- Audio Toolbox
-  AudioComponentCopyIcon(\_:) 

Function

# AudioComponentCopyIcon(\_:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func AudioComponentCopyIcon(_ comp: AudioComponent) -> UIImage?
```

**macOS**

``` source
func AudioComponentCopyIcon(_ comp: AudioComponent) -> NSImage?
```

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

func AudioComponentCopyConfigurationInfo(AudioComponent, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

struct AudioComponentPlugInInterface

typealias AudioComponentMethod

