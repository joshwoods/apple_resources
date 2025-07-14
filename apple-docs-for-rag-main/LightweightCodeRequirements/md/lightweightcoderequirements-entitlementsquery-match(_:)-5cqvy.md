

- LightweightCodeRequirements
- EntitlementsQuery
-  match(\_:) 

Instance Method

# match(\_:)

Match the specified string value against a string or an array of strings.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
func match(_ value: String) -> EntitlementsQuery
```

## Discussion

Strings are matched byte for byte (i.e. no unicode normalization occurs).

