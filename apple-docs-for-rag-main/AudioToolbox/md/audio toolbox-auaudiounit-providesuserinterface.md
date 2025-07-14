

- Audio Toolbox
- AUAudioUnit
-  providesUserInterface 

Instance Property

# providesUserInterface

A Boolean that indicates whether the audio unit provides a user interface, normally in the form of a view controller.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var providesUserInterface: Bool { get }
```

## See Also

### Configuring the User Interface

func supportedViewConfigurations([AUAudioUnitViewConfiguration]) -> IndexSet

func select(AUAudioUnitViewConfiguration)

