

- Core ML
-  MLKey 

Class

# MLKey

An abstract base class for machine learning key types.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class MLKey
```

## Overview

You don’t create use this class directly. Instead, use a class that inherits from this one, such as MLParameterKey or MLMetricKey.

## Topics

### Retrieving a Key’s Information

var name: String

The name of the machine learning key.

var scope: String?

The applicable scope of the machine learning key.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MLMetricKey
- MLParameterKey

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Supporting Types

class MLModelConfiguration

The settings for creating or updating a machine learning model.

struct MLOptimizationHints

