

- AppKit
- Images and PDF
- NSImage
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review symbols that are no longer supported, and find the replacements to use instead.

## Topics

### Class Methods

class func imageFileTypes() -> [String]

Returns an array of strings identifying the image types supported by the registered image representation objects.

Deprecated

class func imageUnfilteredFileTypes() -> [String]

Returns an array of strings identifying the file types supported directly by the registered image representation objects.

Deprecated

class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

### Instance Methods

func lockFocus()

Prepares the image to receive drawing commands.

Deprecated

func lockFocusFlipped(Bool)

Prepares the image to receive drawing commands using the specified flipped state.

Deprecated

func unlockFocus()

Removes the focus from the image.

Deprecated

convenience init(iconRef: IconRef)

Initializes the image object with a Carbon-style icon resource.

Deprecated

