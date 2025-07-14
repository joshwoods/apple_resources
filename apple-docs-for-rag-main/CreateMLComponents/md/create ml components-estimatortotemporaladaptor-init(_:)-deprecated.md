

- Create ML Components
- EstimatorToTemporalAdaptor
-  init(\_:) Deprecated

Initializer

# init(\_:)

Creates a temporal estimator from an estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
init(_ base: Base)
```

## Discussion

The resulting estimator collects all elements of the input sequence before calling fit on the underlying estimator. The transformer returned from fit is also converted to a temporal transformer.

