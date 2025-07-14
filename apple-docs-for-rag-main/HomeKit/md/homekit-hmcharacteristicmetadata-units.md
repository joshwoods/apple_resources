

- HomeKit
- HMCharacteristicMetadata
-  units 

Instance Property

# units

The units of the characteristic value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var units: String? { get }
```

## Discussion

The units property tells you how to use the corresponding characteristic’s value in calculations or how to format it for presentation. For example, you can extend the HMCharacteristic class with a computed property that returns the appropriate symbol to accompany the value in printed output:

```
extension HMCharacteristic {
    var symbol: String {
        guard let units = metadata?.units else { return "" }

        switch units {
        case HMCharacteristicMetadataUnitsPercentage:              return "%"
        case HMCharacteristicMetadataUnitsPartsPerMillion:         return "ppm"
        case HMCharacteristicMetadataUnitsCelsius:                 return "°C"
        case HMCharacteristicMetadataUnitsFahrenheit:              return "°F"
        case HMCharacteristicMetadataUnitsSeconds:                 return "s"
        case HMCharacteristicMetadataUnitsLux:                     return "lx"
        case HMCharacteristicMetadataUnitsMicrogramsPerCubicMeter: return "μg/m³"
        case HMCharacteristicMetadataUnitsArcDegree:               return "°"
        default:                                                   return ""
        }
    }
}
```

See Characteristic Units for the complete list of possible units.

## See Also

### Specifying units

Characteristic Units

Descriptions of the units of a characteristic.

