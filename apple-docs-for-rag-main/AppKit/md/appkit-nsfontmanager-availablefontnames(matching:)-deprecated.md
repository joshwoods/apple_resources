

- AppKit
- NSFontManager
-  availableFontNames(matching:) Deprecated

Instance Method

# availableFontNames(matching:)

Returns the names of the fonts that match the attributes in the given font descriptor.

macOS 10.0–10.11Deprecated

``` source
func availableFontNames(matching descriptor: NSFontDescriptor) -> [Any]?
```

Deprecated

Use `NSFontDescriptor` method matchingFontDescriptors(withMandatoryKeys:) instead.

## Parameters 

`descriptor`  

The font descriptor whose attributes are matched.

## Return Value

The names of the matching fonts.

## See Also

### Methods

func fontDescriptors(inCollection: String) -> [Any]?

Returns an array of the font descriptors in the specified collection.

Deprecated

func addCollection(String, options: NSFontCollectionOptions) -> Bool

Adds a specified font collection to the font manager with a given set of options.

Deprecated

func removeCollection(String) -> Bool

Removes the specified font collection.

Deprecated

func addFontDescriptors([Any], toCollection: String)

Adds an array of font descriptors to the specified font collection.

Deprecated

func removeFontDescriptor(NSFontDescriptor, fromCollection: String)

Removes the specified font descriptor from the specified collection.

Deprecated

func fontManager(_ sender: Any, willIncludeFont fontName: String) -> Bool

Requests permission from the Font panel delegate to display the given font name in the Font panel.

Deprecated

