

- TipKit
- Tips
-  Tips.IgnoresDisplayFrequency 

Structure

# Tips.IgnoresDisplayFrequency

Controls whether a tip obeys the preconfigured display frequency interval.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct IgnoresDisplayFrequency
```

## Overview

Use this option to allow a tip to appear even if the displayFrequency(_:) has not been satisfied.

The default value of this option is false.

```
struct FavoriteBackyardTip: Tip {
    var options: [any Option] {
        IgnoresDisplayFrequency(true)
    }
}
```

## Topics

### Initializers

init(Bool)

## Relationships

### Conforms To

- Sendable
- TipOption

## See Also

### Options

struct MaxDisplayCount

Specifies the maximum number of times a tip displays before the system automatically invalidates it.

struct ConfigurationOption

A type that marks an object as a tip configuration.

struct ParameterOption

A type that represents the various customizations that you can make to a tip parameter.

