

- SensorKit
-  SRSupplementalCategory 

Class

# SRSupplementalCategory

A more detailed category that provides additional context to the app category.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
class SRSupplementalCategory
```

## Overview

This category provides more information about the app while keeping its identity private.

## Topics

### Identifying the Category

var identifier: String

A unique identifier for the supplemental category.

## Relationships

### Inherits From

- NSObject

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
- Sendable

## See Also

### Identifying the App

var bundleIdentifier: String?

The bundle identifier of the app in use.

var reportApplicationIdentifier: String

A pseudonymn for a real application identifier.

var supplementalCategories: [SRSupplementalCategory]

Categories that provide more information about an app.

