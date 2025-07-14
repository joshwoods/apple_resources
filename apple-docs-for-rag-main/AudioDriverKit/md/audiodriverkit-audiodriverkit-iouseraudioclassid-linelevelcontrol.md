

- AudioDriverKit
- AudioDriverKit
- IOUserAudioClassID
-  LineLevelControl 

Enumeration Case

# LineLevelControl

The identifier for the audio line level control class.

DriverKit 21.0+

``` source
LineLevelControl
```

## Discussion

This class is a subclass of the IOUserAudioSelectorControl class that identifies the nominal line level for the element. This control isn’t a gain stage, but instead indicates the voltage standard (if any) used for the element, such as +4dBu, -10dBV, instrument, and so on.

## See Also

### Selector Controls

SelectorControl

The identifier for the audio selector control class.

DataDestinationControl

The identifier for the audio data destination control class.

DataSourceControl

The identifier for the audio data source control class.

ClockSourceControl

The identifier for the audio clock source control class.

HighPassFilterControl

The identifier for the audio high pass filter control class.

