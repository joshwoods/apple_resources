

- Audio Toolbox
-  AudioComponentInstanceCanDo(\_:\_:) 

Function

# AudioComponentInstanceCanDo(\_:\_:)

Determines if an audio component instance implements a particular function.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioComponentInstanceCanDo(
    _ inInstance: AudioComponentInstance,
    _ inSelectorID: Int16
) -> Bool
```

## Parameters 

`inInstance`  

The audio component instance that you want to examine.

`inSelectorID`  

An audio component function selector. The available values for audio units are listed in General Audio Unit Function Selectors and I/O Audio Unit Function Selectors.

## See Also

### Getting Information About a Component

func AudioComponentGetDescription(AudioComponent, UnsafeMutablePointer&lt;AudioComponentDescription>) -> OSStatus

Gets the class description, as an `AudioComponentDescription` structure, of an audio component.

func AudioComponentCopyName(AudioComponent, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Returns the generic name of an audio component.

func AudioComponentGetVersion(AudioComponent, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the version of an audio component in hexadecimal form as `0xMMMMmmDD` (major, minor, dot).

func AudioComponentCopyIcon(AudioComponent) -> UIImage?

func AudioComponentCopyConfigurationInfo(AudioComponent, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

struct AudioComponentPlugInInterface

typealias AudioComponentMethod

