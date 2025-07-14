

- Core Media
- CMFormatDescription
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Equality is derived from

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func == (lhs: CMFormatDescription, rhs: CMFormatDescription) -> Bool
```

## Discussion

```
lhs.equalTo(rhs,
            extensionKeysToIgnore: [],
            sampleDescriptionExtensionAtomKeysToIgnore: [])
```

## See Also

### Comparing Format Descriptions

func equalTo(CMAudioFormatDescription, equalityMask: CMFormatDescription.EqualityMask) -> (Bool, equalityMask: CMFormatDescription.EqualityMask)

Evaluates equality for the parts of two audio format descriptions.

func equalTo(CMFormatDescription, extensionKeysToIgnore: [CMFormatDescription.Extensions.Key], sampleDescriptionExtensionAtomKeysToIgnore: [String]) -> Bool

Evaluates equality for the parts of two audio format descriptions, ignoring the extensions you specify.

