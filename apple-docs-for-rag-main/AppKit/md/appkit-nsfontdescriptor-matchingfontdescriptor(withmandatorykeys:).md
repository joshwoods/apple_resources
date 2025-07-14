

- AppKit
- NSFontDescriptor
-  matchingFontDescriptor(withMandatoryKeys:) 

Instance Method

# matchingFontDescriptor(withMandatoryKeys:)

Returns a normalized font descriptor whose specified attributes match those of the receiver.

macOS 10.5+

``` source
func matchingFontDescriptor(withMandatoryKeys mandatoryKeys: Set?) -> NSFontDescriptor?
```

## Parameters 

`mandatoryKeys`  

Keys that must be identical to be matched. Can be `nil`.

## Return Value

The matching font descriptor. If there is no font that matches the given mandatory key values, returns `nil`.

## Discussion

If more than one font matches the \[`NSFontNameAttribute`, `NSFontFamilyAttribute`, `NSFontVisibleNameAttribute`, `NSFontFaceAttribute`\] attributes, the list of font descriptors is filtered by the other mandatory keys, if any, and the top result that is returned is the same as the first element returned from matchingFontDescriptors(withMandatoryKeys:).

Note

If only one font matches the \[`NSFontNameAttribute`, `NSFontFamilyAttribute`, `NSFontVisibleNameAttribute`, `NSFontFaceAttribute`\] attributes, the `matchingFontDescriptorWithMandatoryKeys:` function returns that font without further filtering for the other mandatory attributes. (This result differs from the result the matchingFontDescriptors(withMandatoryKeys:) function would return.)

In other words, if there is exactly one match with the `NSFontNameAttribute`, `NSFontFamilyAttribute`, `NSFontVisibleNameAttribute`, `NSFontFaceAttribute` attributes, the `matchingFontDescriptorWithMandatoryKeys:` function always returns the font, even if the font doesn’t match the other mandatory keys.

## See Also

### Finding Fonts

func matchingFontDescriptors(withMandatoryKeys: Set&lt;NSFontDescriptor.AttributeName>?) -> [NSFontDescriptor]

Returns all the fonts available on the system whose specified attributes match those of the receiver.

