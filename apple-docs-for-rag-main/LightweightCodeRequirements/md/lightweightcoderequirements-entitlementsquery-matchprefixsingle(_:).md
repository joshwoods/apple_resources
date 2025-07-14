

- LightweightCodeRequirements
- EntitlementsQuery
-  matchPrefixSingle(\_:) 

Instance Method

# matchPrefixSingle(\_:)

Match the specified string prefix value against a string value (not an array).

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
func matchPrefixSingle(_ value: String) -> EntitlementsQuery
```

## Discussion

Strings are matched byte for byte (i.e. no unicode normalization occurs).

