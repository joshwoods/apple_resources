

- Core Image
- CIFilter
-  Filter Attribute Keys 

API Collection

# Filter Attribute Keys

Attributes for a filter and its parameters.

## Overview

Attribute keys are used for the attribute dictionary of a filter. Most entries in the attribute dictionary are optional. The attribute kCIAttributeFilterName is mandatory. For a parameter, the attribute kCIAttributeClass is mandatory because it specifies the class name of the filter.

A parameter of type NSNumber does not necessarily need the attributes kCIAttributeMin and kCIAttributeMax. These attributes are not present when the parameter has no upper or lower bounds. For example, the Gaussian blur filter has a radius parameter with a minimum of `0` but no maximum value to indicate that all nonnegative values are valid.

## Topics

### Constants

let kCIAttributeFilterName: String

The filter name, specified as an NSString object.

let kCIAttributeFilterDisplayName: String

The localized version of the filter name that is displayed in the user interface.

let kCIAttributeDescription: String

The localized description of the filter. This description should inform the user what the filter does and be short enough to display in the user interface for the filter. It is not intended to be technically detailed.

let kCIAttributeFilterAvailable_Mac: String

The macOS version in which the filter first became available, specified as an NSString object.

let kCIAttributeFilterAvailable_iOS: String

The iOS version in which the filter first became available, specified as an NSString object.

let kCIAttributeReferenceDocumentation: String

The localized reference documentation for the filter. The reference should provide developers with technical details.

let kCIAttributeFilterCategories: String

An array of filter category keys that specifies all the categories in which the filter is a member.

let kCIAttributeClass: String

The class name of the filter.

let kCIAttributeType: String

One of the attribute types described in Data Type Attributes.

let kCIAttributeMin: String

The minimum value for a filter parameter, specified as a floating-point value.

let kCIAttributeMax: String

The maximum value for a filter parameter, specified as a floating-point value.

let kCIAttributeSliderMin: String

The minimum value, specified as a floating-point value, to use for a slider that controls input values for a filter parameter.

let kCIAttributeSliderMax: String

The maximum value, specified as a floating-point value, to use for a slider that controls input values for a filter parameter.

let kCIAttributeDefault: String

The default value, specified as a floating-point value, for a filter parameter.

let kCIAttributeIdentity: String

If supplied as a value for a parameter, the parameter has no effect on the input image.

let kCIAttributeName: String

The name of the attribute.

let kCIAttributeDisplayName: String

The localized display name of the attribute.

