

- HomeKit
-  HMAccessoryCategory 

Class

# HMAccessoryCategory

A category for a HomeKit accessory.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMAccessoryCategory
```

## Overview

A category represents a class of devices, like light bulbs or outlets. You can use a category to help users identify the types of accessories they’re browsing. For example, when adding a lamp and a fan to a home, users might not be able to distinguish these accessories if you display only the manufacturer name and model number for each accessory. To improve the user experience, you can use the category information associated with each accessory to help the user understand which accessory is the lamp and which is the fan.

## Topics

### Reading the category type

var categoryType: String

The category to which this accessory belongs.

Accessory Category Types

The accessory category types supported by HomeKit.

### Describing the category

var localizedDescription: String

A localized description of the category.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Categorizing an accessory

var category: HMAccessoryCategory

The category to which the accessory belongs.

