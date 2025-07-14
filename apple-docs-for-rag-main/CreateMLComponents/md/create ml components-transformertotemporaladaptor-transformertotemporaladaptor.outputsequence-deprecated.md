

- Create ML Components
- TransformerToTemporalAdaptor
-  TransformerToTemporalAdaptor.OutputSequence Deprecated

Type Alias

# TransformerToTemporalAdaptor.OutputSequence

The output sequence type.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
typealias OutputSequence = AnyTemporalSequence.Output>
```

## See Also

### Applying

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> AnyTemporalSequence&lt;TransformerToTemporalAdaptor&lt;Base>.Output>

Performs the transformation on each element of the input sequence.

Deprecated

typealias Input

The input type.

Deprecated

typealias Output

The output type.

Deprecated

