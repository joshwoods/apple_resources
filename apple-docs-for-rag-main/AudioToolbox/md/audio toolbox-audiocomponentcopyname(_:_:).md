

- Audio Toolbox
-  AudioComponentCopyName(\_:\_:) 

Function

# AudioComponentCopyName(\_:\_:)

Returns the generic name of an audio component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentCopyName(
    _ inComponent: AudioComponent,
    _ outName: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`inComponent`  

The audio component that you want the generic name of.

`outName`  

On output, the generic name of the specified audio component.

## Return Value

A result code.

## See Also

### Getting Information About a Component

func AudioComponentInstanceCanDo(AudioComponentInstance, Int16) -> Bool

Determines if an audio component instance implements a particular function.

func AudioComponentGetDescription(AudioComponent, UnsafeMutablePointer&lt;AudioComponentDescription>) -> OSStatus

Gets the class description, as an `AudioComponentDescription` structure, of an audio component.

func AudioComponentGetVersion(AudioComponent, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the version of an audio component in hexadecimal form as `0xMMMMmmDD` (major, minor, dot).

func AudioComponentCopyIcon(AudioComponent) -> UIImage?

func AudioComponentCopyConfigurationInfo(AudioComponent, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

struct AudioComponentPlugInInterface

typealias AudioComponentMethod

