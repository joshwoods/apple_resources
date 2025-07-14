

- AppKit
-  Images and PDF 

API Collection

# Images and PDF

Create and manage images, in bitmap, PDF, and other formats.

## Topics

### Images

Providing images for different appearances

Supply image resources appropriate for light and dark appearances and for high-contrast environments.

Supporting Continuity Camera in Your Mac App

Incorporate scanned documents and pictures from a user’s iPhone, iPad, or iPod touch into your Mac app using Continuity Camera.

Supporting HDR images in your app

​Load, display, edit, and save HDR images using SwiftUI and Core Image. ​

Applying Apple HDR effect to your photos

You can decode and apply Apple’s HDR gain map to your own images.

class NSImage

A high-level interface for manipulating image data.

protocol NSImageDelegate

A set of optional methods that you can use to respond to drawing failures and manage incremental loads.

class NSImageRep

A semiabstract superclass that provides subclasses that you use to draw an image from a particular type of source data.

### Bitmap Formats

class NSBitmapImageRep

An object that renders an image from bitmap data.

class NSCIImageRep

An object that can render an image from a Core Image object.

class NSPICTImageRep

An object that renders an image from a PICT format data stream of version 1, version 2, and extended version 2.

### Vector Formats

class NSPDFImageRep

An object that can render an image from a PDF format data stream.

class NSPDFInfo

An object that stores information associated with the creation of a PDF file, such as its URL, tag names, page orientation, and paper size.

class NSEPSImageRep

An object that can render an image from encapsulated PostScript (EPS) code.

Deprecated

### Custom Formats

class NSCustomImageRep

An object that uses a delegate object to render an image from a custom format.

## See Also

### Graphics, Drawing, Color, and Printing

Drawing

Draw shapes, images, and other content on the screen.

Color

Represent colors using built-in or custom formats, and give users options for selecting and applying colors.

Printing

Display the system print panels and manage the printing process.

