

- Quartz
- QCCompositionRenderer
-  attributes() Deprecated

Instance Method

# attributes()

Returns the attributes of the composition associated with the renderer.

macOS 10.4–10.15Deprecated

``` source
func attributes() -> [AnyHashable : Any]!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A dictionary that contains the attributes that describe the composition, including the input and output ports of the root patch.

## Discussion

The dictionary can define any of the attributes that are specified by the composition attribute keys. See QCCompositionAttributeNameKey, QCCompositionAttributeDescriptionKey, and QCCompositionAttributeCopyrightKey.

The dictionary can also contain dictionaries that correspond to the keys that identify the input and output ports of the root patch of the composition. See QCPortAttributeTypeKey, QCPortAttributeNameKey, QCPortAttributeMinimumValueKey, QCPortAttributeMaximumValueKey, and QCPortAttributeMenuItemsKey.

## See Also

### Related Documentation

func inputKeys() -> [Any]!

Returns an array that contains the keys that identify the input ports of the root patch of the composition.

**Required**

Deprecated

func outputKeys() -> [Any]!

Returns an array that contains the keys that identify the output ports of the root patch of the composition.

**Required**

Deprecated

