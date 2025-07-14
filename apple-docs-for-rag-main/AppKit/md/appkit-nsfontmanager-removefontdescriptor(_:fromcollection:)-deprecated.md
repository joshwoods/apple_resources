

- AppKit
- NSFontManager
-  removeFontDescriptor(\_:fromCollection:) Deprecated

Instance Method

# removeFontDescriptor(\_:fromCollection:)

Removes the specified font descriptor from the specified collection.

macOS 10.0–10.11Deprecated

``` source
func removeFontDescriptor(
    _ descriptor: NSFontDescriptor,
    fromCollection collection: String
)
```

Deprecated

Use removeQuery(for:) instead.

## Parameters 

`descriptor`  

The font descriptor to remove.

`collection`  

The font collection from which to remove the descriptor.

## See Also

### Methods

func availableFontNames(matching: NSFontDescriptor) -> [Any]?

Returns the names of the fonts that match the attributes in the given font descriptor.

Deprecated

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

func fontManager(_ sender: Any, willIncludeFont fontName: String) -> Bool

Requests permission from the Font panel delegate to display the given font name in the Font panel.

Deprecated

