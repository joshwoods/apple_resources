

- Create ML Components
- TransformerToTemporalAdaptor
-  applied(to:eventHandler:) Deprecated

Instance Method

# applied(to:eventHandler:)

Performs the transformation on each element of the input sequence.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func applied(
    to input: S,
    eventHandler: EventHandler? = nil
) async throws -> AnyTemporalSequence.Output> where S : TemporalSequence, Base.Input == S.Feature
```

## See Also

### Applying

typealias Input

The input type.

Deprecated

typealias Output

The output type.

Deprecated

typealias OutputSequence

The output sequence type.

Deprecated

