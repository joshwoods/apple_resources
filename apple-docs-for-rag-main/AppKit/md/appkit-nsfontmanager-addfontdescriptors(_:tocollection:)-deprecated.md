

- AppKit
- NSFontManager
-  addFontDescriptors(\_:toCollection:) Deprecated

Instance Method

# addFontDescriptors(\_:toCollection:)

Adds an array of font descriptors to the specified font collection.

macOS 10.0–10.11Deprecated

``` source
func addFontDescriptors(
    _ descriptors: [Any],
    toCollection collectionName: String
)
```

Deprecated

Use addQuery(for:) instead.

## Parameters 

`descriptors`  

The font descriptors to add.

`collectionName`  

The font collection to which descriptors are added.

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

func removeFontDescriptor(NSFontDescriptor, fromCollection: String)

Removes the specified font descriptor from the specified collection.

Deprecated

func fontManager(_ sender: Any, willIncludeFont fontName: String) -> Bool

Requests permission from the Font panel delegate to display the given font name in the Font panel.

Deprecated

