

- LightweightCodeRequirements
- EntitlementsQuery
-  matchPrefix(\_:) 

Instance Method

# matchPrefix(\_:)

Match the specified string prefix against a string value or array.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
func matchPrefix(_ value: String) -> EntitlementsQuery
```

## Discussion

Strings are matched byte for byte (i.e. no unicode normalization occurs). matchPrefix will match only the first string value that has the prefix.

