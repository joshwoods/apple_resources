

- PHASE
- PHASESpatialCategory
-  init(rawValue:) 

Initializer

# init(rawValue:)

Initializes a spatial category with the given string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(rawValue: String)
```

## Parameters 

`rawValue`  

The enumeration case’s underlying string value.

## Discussion

To initialize a spatial category:

```
// Set the raw-value variable to the `directPathTransmission` constant. 
var rawValue: String = PHASESpatialCategoryDirectPathTransmission
var spatialPipelineOption = PHASESpatialCategory(rawValue: rawValue)
```

To check a spatial category’s raw value, see the Objective-C declaration of the struct member.

