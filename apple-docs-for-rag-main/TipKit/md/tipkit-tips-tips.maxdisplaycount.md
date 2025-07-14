

- TipKit
- Tips
-  Tips.MaxDisplayCount 

Structure

# Tips.MaxDisplayCount

Specifies the maximum number of times a tip displays before the system automatically invalidates it.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct MaxDisplayCount
```

## Overview

Use this option to automatically invalidate a tip after it has appeared a specified number of times.

By default tips have no maximum display count.

```
struct FavoriteBackyardTip: Tip {
    var options: [any Option] {
        // Tip will only appear 3 times before it is automatically invalidated.
        MaxDisplayCount(3)
    }
}
```

## Topics

### Initializers

init(Int)

## Relationships

### Conforms To

- Sendable
- TipOption

## See Also

### Options

struct IgnoresDisplayFrequency

Controls whether a tip obeys the preconfigured display frequency interval.

struct ConfigurationOption

A type that marks an object as a tip configuration.

struct ParameterOption

A type that represents the various customizations that you can make to a tip parameter.

