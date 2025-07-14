

- Observation
-  Observable 

Protocol

# Observable

A type that emits notifications to observers when underlying data changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol Observable
```

## Mentioned in 

Applying Macros

## Overview

Conforming to this protocol signals to other APIs that the type supports observation. However, applying the `Observable` protocol by itself to a type doesn’t add observation functionality to the type. Instead, always use the Observable() macro when adding observation support to a type.

## See Also

### Observable conformance

macro Observable()

Defines and implements conformance of the Observable protocol.

