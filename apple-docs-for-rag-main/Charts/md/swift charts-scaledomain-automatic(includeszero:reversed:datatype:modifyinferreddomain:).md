

- Swift Charts
- ScaleDomain
-  automatic(includesZero:reversed:dataType:modifyInferredDomain:) 

Type Method

# automatic(includesZero:reversed:dataType:modifyInferredDomain:)

Creates a scale domain configuration that infers the scale domain from data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func automatic(
    includesZero: Bool? = nil,
    reversed: Bool? = nil,
    dataType: DataValue.Type,
    modifyInferredDomain: @escaping (inout [DataValue]) -> Void
) -> AutomaticScaleDomain where DataValue : Plottable
```

Available when `Self` is `AutomaticScaleDomain`.

## Parameters 

`includesZero`  

Whether the scale domain should include zero (only applicable for numerical values).

`reversed`  

Whether the scale domain should be reversed (e.g., 100 … 0).

`dataType`  

The type of a data value in the domain.

`modifyInferredDomain`  

A closure that modifies the automatically inferred domain.

## Discussion

You can modify the inferred scale domain with a function.

For instance, you can sort the categories in a categorical x scale:

```
Chart { ... }
.chartXScale(domain: .automatic(dataType: String.self) { domain in
    // Sort the categories.
    domain.sort(using: .localizedStandard)
    // Include a new category.
    domain.append("Other")
}
```

You can also modify a numerical scale to include a given value. The example below sets the y scale to always include the value 100.

```
Chart { ... }
.chartYScale(domain: .automatic(dataType: Double.self) { domain in
    domain.append(100)
}
```

Note that the `modifyInferredDomain` closure is used as part of the automatic scale domain inference process. The result of it can be further modified by the `reversed` parameter, and to include values from axis marks. To set the scale domain to an exact value, specify the value as the `domain:` argument directly instead of using `.automatic`.

