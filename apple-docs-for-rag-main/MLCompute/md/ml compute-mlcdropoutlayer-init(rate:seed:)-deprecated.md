

- ML Compute
- MLCDropoutLayer
-  init(rate:seed:) Deprecated

Initializer

# init(rate:seed:)

Creates a dropout layer with the probability rate and random number generator seed you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    rate: Float,
    seed: Int
)
```

## Parameters 

`rate`  

The dropout rate you use for each element.

`seed`  

The seed you use to generate random numbers.

