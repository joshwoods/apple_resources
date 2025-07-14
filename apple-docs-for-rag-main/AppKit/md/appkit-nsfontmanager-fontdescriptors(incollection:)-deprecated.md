

- AppKit
- NSFontManager
-  fontDescriptors(inCollection:) Deprecated

Instance Method

# fontDescriptors(inCollection:)

Returns an array of the font descriptors in the specified collection.

macOS 10.0–10.11Deprecated

``` source
func fontDescriptors(inCollection collectionNames: String) -> [Any]?
```

Deprecated

Use matchingDescriptors instead.

## Parameters 

`collectionNames`  

The font collection for which to return descriptors.

## Return Value

The font descriptors.

## See Also

### Related Documentation

var collectionNames: [Any]

The names of the currently loaded font collections.

Deprecated

### Methods

func availableFontNames(matching: NSFontDescriptor) -> [Any]?

Returns the names of the fonts that match the attributes in the given font descriptor.

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

