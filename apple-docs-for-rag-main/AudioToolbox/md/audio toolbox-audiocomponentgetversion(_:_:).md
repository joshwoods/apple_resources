

- Audio Toolbox
-  AudioComponentGetVersion(\_:\_:) 

Function

# AudioComponentGetVersion(\_:\_:)

Gets the version of an audio component in hexadecimal form as `0xMMMMmmDD` (major, minor, dot).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentGetVersion(
    _ inComponent: AudioComponent,
    _ outVersion: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inComponent`  

The audio component that you want the version of.

`outVersion`  

The version of the specified audio component.

## Return Value

A result code.

## See Also

### Getting Information About a Component

func AudioComponentInstanceCanDo(AudioComponentInstance, Int16) -> Bool

Determines if an audio component instance implements a particular function.

func AudioComponentGetDescription(AudioComponent, UnsafeMutablePointer&lt;AudioComponentDescription>) -> OSStatus

Gets the class description, as an `AudioComponentDescription` structure, of an audio component.

func AudioComponentCopyName(AudioComponent, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Returns the generic name of an audio component.

func AudioComponentCopyIcon(AudioComponent) -> UIImage?

func AudioComponentCopyConfigurationInfo(AudioComponent, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

struct AudioComponentPlugInInterface

typealias AudioComponentMethod

