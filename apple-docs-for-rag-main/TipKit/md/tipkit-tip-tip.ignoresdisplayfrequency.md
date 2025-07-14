

- TipKit
- Tip
-  Tip.IgnoresDisplayFrequency 

Type Alias

# Tip.IgnoresDisplayFrequency

Controls whether a tip obeys the preconfigured display frequency interval.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
typealias IgnoresDisplayFrequency = Tips.IgnoresDisplayFrequency
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

## See Also

### Tip options

typealias MaxDisplayCount

Specifies the maximum number of times a tip displays before the system automatically invalidates it.

typealias MaxDisplayDuration

Specifies the maximum amount of time a tip is displayed before it is invalidated.

