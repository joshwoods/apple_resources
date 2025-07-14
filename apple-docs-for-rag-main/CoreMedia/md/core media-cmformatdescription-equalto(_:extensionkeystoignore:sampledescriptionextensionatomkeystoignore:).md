

- Core Media
- CMFormatDescription
-  equalTo(\_:extensionKeysToIgnore:sampleDescriptionExtensionAtomKeysToIgnore:) 

Instance Method

# equalTo(\_:extensionKeysToIgnore:sampleDescriptionExtensionAtomKeysToIgnore:)

Evaluates equality for the parts of two audio format descriptions, ignoring the extensions you specify.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func equalTo(
    _ otherFormatDescription: CMFormatDescription,
    extensionKeysToIgnore: [CMFormatDescription.Extensions.Key] = [],
    sampleDescriptionExtensionAtomKeysToIgnore: [String] = []
) -> Bool
```

## Parameters 

`otherFormatDescription`  

A format description to compare to.

`extensionKeysToIgnore`  

A list of format description extension keys.

`sampleDescriptionExtensionAtomKeysToIgnore`  

A list of sample description extension atom keys.

## See Also

### Comparing Format Descriptions

static func == (CMFormatDescription, CMFormatDescription) -> Bool

Equality is derived from

func equalTo(CMAudioFormatDescription, equalityMask: CMFormatDescription.EqualityMask) -> (Bool, equalityMask: CMFormatDescription.EqualityMask)

Evaluates equality for the parts of two audio format descriptions.

