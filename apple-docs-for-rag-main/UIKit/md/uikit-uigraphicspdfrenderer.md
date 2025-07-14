

- UIKit
-  UIGraphicsPDFRenderer 

Class

# UIGraphicsPDFRenderer

A graphics renderer for creating PDFs.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsPDFRenderer
```

## Overview

You can use PDF renderers to create PDF files, without having to manage Core Graphics contexts.

To render a PDF:

1.  Optionally create a UIGraphicsPDFRendererFormat object to specify nondefault parameters the renderer should use to create its context.

2.  Instantiate a UIGraphicsPDFRenderer object, providing the dimensions of the output image and a format object. The renderer uses sensible defaults for the current device if you don’t provide format object, as demonstrated in Creating a graphics PDF renderer.

3.  Choose one of the rendering methods depending on your desired output: pdfData(actions:) outputs the PDF in the form of a Data object, and writePDF(to:withActions:) saves the PDF as a file directly to disk.

4.  Provide Core Graphics drawing instructions within the closure associated with your chosen method, as shown in Creating a PDF with a PDF renderer.

5.  Optionally, you can create a multi-page PDF, using the approach shown in Adding pages.

6.  Optionally, add links to your PDF to make navigation easy, as shown in Creating internal links.

After initializing a PDF renderer, you can use it to draw multiple PDFs with the same configuration.

### Creating a graphics PDF renderer

Create a PDF renderer, providing the bounds of the PDF page.

- Swift
- Objective-C

```
let renderer = UIGraphicsPDFRenderer(bounds: CGRect(x: 0, y: 0, width: 500, height: 300))
```

```
UIGraphicsPDFRenderer *renderer = [[UIGraphicsPDFRenderer alloc] initWithBounds:CGRectMake(0, 0, 500, 300)];
```

You can instead use one of the other UIGraphicsPDFRenderer initializers to specify a renderer format (UIGraphicsPDFRendererFormat) in addition to the bounds. This allows you to configure the underlying Core Graphics context with custom PDF document info. If you don’t provide a format, the renderer uses the default() format, which creates a context best suited for the current device.

### Creating a PDF with a PDF renderer

Use the pdfData(actions:) method to create a PDF with the PDF renderer you created above. This takes a block that represents the drawing actions. Within this block, the renderer creates a Core Graphics context using the parameters provided during renderer initialization, and sets this to be the current context.

Before issuing PDF drawing instructions, you must create a page with a call to either the beginPage() method or beginPage(withBounds:pageInfo:) method on the supplied UIGraphicsPDFRendererContext.

- Swift
- Objective-C

```
let pdf = renderer.pdfData { (context) in
  context.beginPage()
  let attributes = [
    NSFontAttributeName : UIFont.boldSystemFont(ofSize: 150)
  ]
  let text = "Hello!" as NSString
  text.draw(in: CGRect(x: 0, y: 0, width: 500, height: 200), withAttributes: attributes)
}
```

```
NSData *pdf = [renderer PDFDataWithActions:^(UIGraphicsPDFRendererContext * _Nonnull context) {
  [context beginPage];
  NSDictionary *attributes = @{NSFontAttributeName : [UIFont boldSystemFontOfSize:150]};
  NSString *text = @"Hello!";
  [text drawInRect:CGRectMake(0, 0, 500, 200) withAttributes:attributes];}];  
```

The drawing actions closure takes a single argument of type UIGraphicsPDFRendererContext. This provides access to some high-level drawing functions, such as fill(_:) through the UIGraphicsRendererContext superclass.

Note

This code uses a drawing method on NSString. If you want to create a PDF with more text, consider using TextKit or Core Text, both of which provide extensive text layout functionality.

The above code creates the following result:

### Adding pages

Add multiple pages to your PDF through repeated calls to the beginPage() method on the UIGraphicsPDFRendererContext provided to the drawing block.

- Swift
- Objective-C

```
let pdf = renderer.pdfData { (context) in
  let attributes = [
    NSFontAttributeName : UIFont.boldSystemFont(ofSize: 150)
  ]
  for page in 1...3 {
    context.beginPage()
    let text = "Page \(page)" as NSString
    text.draw(in: CGRect(x: 0, y: 0, width: 500, height: 200), withAttributes: attributes)
  }
}
```

```
NSData *pdf = [renderer PDFDataWithActions:^(UIGraphicsPDFRendererContext * _Nonnull context) {
  NSDictionary *attributes = @{NSFontAttributeName : [UIFont boldSystemFontOfSize:150]}; 
  for (int page = 1; page 

Use the beginPage(withBounds:pageInfo:) method instead of the beginPage() method if you want to override the default properties for the new page.

This code creates a PDF with three pages, each of which contains the current page number as large text, as shown in the following image.

### Creating internal links

You can create internal links, known as destinations, in PDFs. A complete link has two components:

- A named destination. This is a point on a PDF page. You create these with the addDestination(withName:at:) method on UIGraphicsPDFRendererContext.

- A link region. This is a rectangle on a PDF page, which when tapped, instructs the PDF viewing app to jump to a specific named destination. You create these with the setDestinationWithName(_:for:) method on UIGraphicsPDFRendererContext, providing the name of the destination to jump to, and the bounds of the active link region.

The following code demonstrates how to use destinations with a PDF renderer by showing how to create links that jump to the next page.

- Swift
- Objective-C

```
let pdf = renderer.pdfData { (context) in
  let pageNumberAttributes = [
    NSFontAttributeName : UIFont.boldSystemFont(ofSize: 150)
  ]

  let nextPage = "Next Page ↠" as NSString
  let nextPageRect = CGRect(x: 350, y: 250, width: 150, height: 40)
  let nextPageAttributes = [
    NSFontAttributeName : UIFont.systemFont(ofSize: 25),
    NSBackgroundColorAttributeName : UIColor.red,
    NSForegroundColorAttributeName : UIColor.white
  ]

  for page in 1...3 {
    context.beginPage()
    let pageNumber = "Page \(page)" as NSString
    pageNumber.draw(in: CGRect(x: 0, y: 0, width: 500, height: 200), withAttributes: pageNumberAttributes)

    nextPage.draw(in: nextPageRect, withAttributes: nextPageAttributes)

    context.addDestination(withName: "page-\(page)", at: CGPoint.zero.applying(context.cgContext.userSpaceToDeviceSpaceTransform))
    context.setDestinationWithName("page-\(page + 1)", for: nextPageRect.applying(context.cgContext.userSpaceToDeviceSpaceTransform))
  }
}
```

```
NSData *pdf = [renderer PDFDataWithActions:^(UIGraphicsPDFRendererContext * _Nonnull context) {
  NSDictionary *attributes = @{NSFontAttributeName : [UIFont boldSystemFontOfSize:150]};

  NSString *nextPage = @"Next Page ↠";
  CGRect nextPageRect = CGRectMake(350, 250, 150, 40);
  NSDictionary *nextPageAttributes = @{
    NSFontAttributeName : [UIFont systemFontOfSize:25],
    NSBackgroundColorAttributeName : [UIColor redColor],
    NSForegroundColorAttributeName : [UIColor whiteColor]
  };
  for (int page = 1; page 

This code adds large red labels that jump from the current page to the next page when clicked. Each page has a destination with names of the form `page-1`, positioned at the origin. The bounding box for the next-page label is the link to the destination on the following page.

Note

The addDestination(withName:at:) and setDestinationWithName(_:for:) methods on UIGraphicsPDFRendererContext use the underlying PDF coordinate space, which has its y-axis flipped with respect to the coordinate system used by Core Graphics. You can translate between the two using the userSpaceToDeviceSpaceTransform property on CGContext, as shown in the code.

The above code results in the following PDF:

## Topics

### Creating a PDF renderer

init(bounds: CGRect, format: UIGraphicsPDFRendererFormat)

Creates a new graphics renderer with the specified bounds and format.

### Managing the PDF data

func pdfData(actions: (UIGraphicsPDFRendererContext) -> Void) -> Data

Creates a PDF from a set of drawing instructions and returns it as a data object.

func writePDF(to: URL, withActions: (UIGraphicsPDFRendererContext) -> Void) throws

Creates a PDF from a set of drawing instructions and saves it to a specified URL.

typealias DrawingActions

A closure for drawing PDF content.

## Relationships

### Inherits From

- UIGraphicsRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Graphics contexts

class UIGraphicsRenderer

An abstract base class for creating graphics renderers.

class UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

class UIGraphicsImageRendererContext

The drawing environment for an image renderer.

class UIGraphicsImageRendererFormat

A set of drawing attributes that represents the configuration of an image renderer context.

class UIGraphicsPDFRendererContext

The drawing environment for a PDF renderer.

class UIGraphicsPDFRendererFormat

A set of drawing attributes that represents the configuration of a PDF renderer context.

