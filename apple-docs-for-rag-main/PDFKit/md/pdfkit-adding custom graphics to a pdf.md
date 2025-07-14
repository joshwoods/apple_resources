

- PDFKit
-  Adding Custom Graphics to a PDF 

Article

# Adding Custom Graphics to a PDF

Create and add custom annotation and page graphics to your PDF document.

## Overview

You can add custom annotation and page graphics to a PDF by overriding the `draw` method for PDFAnnotation or PDFPage. If the graphic applies to the whole page, like a watermark, custom border, or logo, you add it to the page using PDFPage. If the graphic is something small, such as circling or highlighting a particular element on the page, or a repeatable custom graphic, such as a heart, club, spade, or diamond, then it should be added using PDFAnnotation. Some graphics, like lines, can work as annotations or page elements.

Drawings are static, unlike interactive annotation types like widgets. To learn more about widgets, see Adding Widgets to a PDF Document.

### Register a Delegate for the Document

Register a PDFDocumentDelegate to the PDFDocument loaded in the current PDFView. This delegate will allow you to specify a method for building PDF annotations or PDF pages. The PDFDocument is called `document`.

```
```

### Implement a Custom Subclass

Create a custom subclass for your custom graphics, one that will include your drawing. This example shows how to add a custom line graphic to a PDF, either through a PDF annotation or a PDF page.

#### Implement a Custom Annotation Subclass

Create a custom annotation subclass for your line graphic.

```
```

Implement the class(forAnnotationType:) function in the document’s delegate. This method returns the subclass type for PDFAnnotation for a given annotation subtype string. In this case you return the `LineAnnotation` class for a `Line` type annotation.

```
```

#### Implement a Custom Page Subclass

Create a custom subclass for PDFPage that includes your line graphic.

```
```

Implement the classForPage() function in the document delegate. This class returns the subclass type for PDFPage, the `LinePage` class:

```
```

### Override the Draw Method and Add Your Custom Graphic

Override the `draw` method in your subclass to draw your custom graphic, the line. Draw the original content by calling the superclass version of the `draw` method. The `draw` methods for pages and annotations are nearly identical, the only difference being the `in context` parameter for annotations and the `to context` parameter for pages:

**For annotations, use this** draw(with:) **method:**

```
```

**For pages, use this** draw(with:) **method:**

```
```

In the appropriate `draw` method, add your custom drawing, in this case the line. To ensure that your drawing maintains its CGContext properties and doesn’t affect other contexts in your PDF, make sure to save and restore your graphics state (before and after, respectively) you add your custom drawing code.

Important

Ensure that you draw your content with respect to the PDF page coordinate system. The origin is at the bottom left corner, with the Y axis increasing from bottom to top and the X axis increasing from left to right.

```
```

Note

PDFAnnotation also allows custom drawing for annotations with a type unknown to PDFKit, but only if the annotation has an appearance stream (hasAppearanceStream).

## See Also

### Annotations

Adding Widgets to a PDF Document

Add text, button, and choice widgets to a PDF document.

Custom Graphics

Demonstrates adding a watermark to a PDF page.

PDF Widgets

Demonstrates adding widgets—interactive form elements—to a PDF document.

class PDFAnnotation

An annotation in a PDF document.

