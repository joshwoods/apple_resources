

- Core Media
- CMFormatDescription
-  equalTo(\_:equalityMask:) 

Instance Method

# equalTo(\_:equalityMask:)

Evaluates equality for the parts of two audio format descriptions.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func equalTo(
    _ otherFormatDescription: CMAudioFormatDescription,
    equalityMask: CMFormatDescription.EqualityMask = .all
) -> (Bool, equalityMask: CMFormatDescription.EqualityMask)
```

## Parameters 

`otherFormatDescription`  

A format description to compare.

`equalityMask`  

A mask that specifies which parts of the descriptions to compare.

## See Also

### Comparing Format Descriptions

static func == (CMFormatDescription, CMFormatDescription) -> Bool

Equality is derived from

func equalTo(CMFormatDescription, extensionKeysToIgnore: [CMFormatDescription.Extensions.Key], sampleDescriptionExtensionAtomKeysToIgnore: [String]) -> Bool

Evaluates equality for the parts of two audio format descriptions, ignoring the extensions you specify.

