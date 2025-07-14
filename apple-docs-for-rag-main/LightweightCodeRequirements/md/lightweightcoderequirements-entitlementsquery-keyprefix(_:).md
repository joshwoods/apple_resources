

- LightweightCodeRequirements
- EntitlementsQuery
-  keyPrefix(\_:) 

Type Method

# keyPrefix(\_:)

Match the specified key prefix at the root of the entitlements dicitonary. Chain additional qualifiers to constrain the value of the key.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static func keyPrefix(_ keyPrefix: String) -> EntitlementsQuery
```

## Discussion

Keys are matched byte for byte (i.e. no unicode normalization occurs). keyPrefix will match only the first key with the prefix. Chained qualifiers will be applied to the value of that single key only.

