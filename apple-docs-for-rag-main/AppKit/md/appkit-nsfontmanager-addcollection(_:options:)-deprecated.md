

- AppKit
- NSFontManager
-  addCollection(\_:options:) Deprecated

Instance Method

# addCollection(\_:options:)

Adds a specified font collection to the font manager with a given set of options.

macOS 10.0–10.11Deprecated

``` source
func addCollection(
    _ collectionName: String,
    options collectionOptions: NSFontCollectionOptions = []
) -> Bool
```

Deprecated

Use show(_:withName:visibility:) instead.

## Parameters 

`collectionName`  

The collection to add.

`collectionOptions`  

The option described in `Font Collection Mask`. This option is not yet implemented.

## Return Value

true if the font collection was successfully added; otherwise, false.

## See Also

### Methods

func availableFontNames(matching: NSFontDescriptor) -> [Any]?

Returns the names of the fonts that match the attributes in the given font descriptor.

Deprecated

func fontDescriptors(inCollection: String) -> [Any]?

Returns an array of the font descriptors in the specified collection.

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

