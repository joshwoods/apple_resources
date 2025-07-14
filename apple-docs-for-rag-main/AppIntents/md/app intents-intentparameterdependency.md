

- App Intents
-  IntentParameterDependency 

Class

# IntentParameterDependency

A property wrapper that represents an app intent dependency you use to provide dynamic options.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@propertyWrapper
final class IntentParameterDependency where Intent : AppIntent
```

## Overview

Use the `IntentParameterDependency` property wrapper for properties that represent dynamic options in your DynamicOptionsProvider implementations as shown in the following example:

```
struct SoupQuery: EntityStringQuery {
    @IntentParameterDependency(
        \.$quantity
    )
    var orderSoup

    func entities(matching string: String) async throws -> [Soup] {
        guard let orderSoup else {
            return []
        }
        return Soup.allSoups.filter {
            $0.name.contains(string) &&
            $0.availableQuantity >= orderSoup.quantity
        }
    }
}
```

## Topics

### Initializers

convenience init&lt;V0, P0>(KeyPath&lt;Intent, P0>)

convenience init&lt;V0, P0, V1, P1>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>)

convenience init&lt;V0, P0, V1, P1, V2, P2>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6, V7, P7>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>, KeyPath&lt;Intent, P7>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6, V7, P7, V8, P8>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>, KeyPath&lt;Intent, P7>, KeyPath&lt;Intent, P8>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6, V7, P7, V8, P8, V9, P9>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>, KeyPath&lt;Intent, P7>, KeyPath&lt;Intent, P8>, KeyPath&lt;Intent, P9>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6, V7, P7, V8, P8, V9, P9, V10, P10>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>, KeyPath&lt;Intent, P7>, KeyPath&lt;Intent, P8>, KeyPath&lt;Intent, P9>, KeyPath&lt;Intent, P10>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6, V7, P7, V8, P8, V9, P9, V10, P10, V11, P11>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>, KeyPath&lt;Intent, P7>, KeyPath&lt;Intent, P8>, KeyPath&lt;Intent, P9>, KeyPath&lt;Intent, P10>, KeyPath&lt;Intent, P11>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6, V7, P7, V8, P8, V9, P9, V10, P10, V11, P11, V12, P12>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>, KeyPath&lt;Intent, P7>, KeyPath&lt;Intent, P8>, KeyPath&lt;Intent, P9>, KeyPath&lt;Intent, P10>, KeyPath&lt;Intent, P11>, KeyPath&lt;Intent, P12>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6, V7, P7, V8, P8, V9, P9, V10, P10, V11, P11, V12, P12, V13, P13>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>, KeyPath&lt;Intent, P7>, KeyPath&lt;Intent, P8>, KeyPath&lt;Intent, P9>, KeyPath&lt;Intent, P10>, KeyPath&lt;Intent, P11>, KeyPath&lt;Intent, P12>, KeyPath&lt;Intent, P13>)

convenience init&lt;V0, P0, V1, P1, V2, P2, V3, P3, V4, P4, V5, P5, V6, P6, V7, P7, V8, P8, V9, P9, V10, P10, V11, P11, V12, P12, V13, P13, V14, P14>(KeyPath&lt;Intent, P0>, KeyPath&lt;Intent, P1>, KeyPath&lt;Intent, P2>, KeyPath&lt;Intent, P3>, KeyPath&lt;Intent, P4>, KeyPath&lt;Intent, P5>, KeyPath&lt;Intent, P6>, KeyPath&lt;Intent, P7>, KeyPath&lt;Intent, P8>, KeyPath&lt;Intent, P9>, KeyPath&lt;Intent, P10>, KeyPath&lt;Intent, P11>, KeyPath&lt;Intent, P12>, KeyPath&lt;Intent, P13>, KeyPath&lt;Intent, P14>)

### Instance Properties

var wrappedValue: IntentProjection&lt;Intent>?

### Default Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Intent parameters

class IntentParameter

A property wrapper that indicates the associated property is an input argument of the app intent.

struct IntentParameterContext

A type that provides information about an associated parameter during value resolution.

enum InputConnectionBehavior

Describes the input behaviors for connecting a parameter to the output of the previous App Intent.

