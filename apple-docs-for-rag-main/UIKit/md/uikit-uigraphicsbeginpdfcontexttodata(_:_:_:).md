

- UIKit
-  UIGraphicsBeginPDFContextToData(\_:\_:\_:) 

Function

# UIGraphicsBeginPDFContextToData(\_:\_:\_:)

Creates a PDF graphics context that targets the specified mutable data object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func UIGraphicsBeginPDFContextToData(
    _ data: NSMutableData,
    _ bounds: CGRect,
    _ documentInfo: [AnyHashable : Any]?
)
```

## Parameters 

`data`  

The data object to receive the PDF output data.

`bounds`  

A rectangle that specifies the default size and location of PDF pages. (This value is used as the default media box for each new page.) The origin of the rectangle should typically be (0, 0). Specifying an empty rectangle (CGRectZero) sets the default page size to 8.5 by 11 inches (612 by 792 points).

`documentInfo`  

A dictionary that specifies additional information to be associated with the PDF file. You can use these keys to specify additional metadata and security information for the PDF, such as the author of the PDF or the password for accessing it. The keys in this dictionary are the same keys you pass to the init(consumer:mediaBox:_:) function and are described in the Auxiliary Dictionary Keys section of doc://com.apple.documentation/documentation/coregraphics/cgpdfcontext. The dictionary is retained by the new context, so on return you may safely release it.

Specify `nil` if you do not want to associate any additional information with the PDF document.

## Discussion

After creating the graphics context, this function makes it the current drawing context. Any subsequent drawing commands are therefore captured and turned into PDF data. When you are done drawing, you must call the UIGraphicsEndPDFContext() function to close the PDF graphics context.

You can use all of the same drawing routines that you would normally use to draw the contents of your application. The graphics context converts all drawing commands into PDF drawing commands automatically. However, before you issue any drawing commands to a PDF context, you must start a new page by calling the UIGraphicsBeginPDFPage() or UIGraphicsBeginPDFPageWithInfo(_:_:) function. You can also use these functions to define additional pages later.

After creating it, you can get the PDF context using the UIGraphicsGetCurrentContext() function.

## See Also

### PDF creation

func UIGraphicsBeginPDFContextToFile(String, CGRect, [AnyHashable : Any]?) -> Bool

Creates a PDF graphics context that targets a file at the specified path.

func UIGraphicsEndPDFContext()

Closes a PDF graphics context and pops it from the current context stack.

func UIGraphicsBeginPDFPage()

Marks the beginning of a new page in a PDF context and configures it using default values.

func UIGraphicsBeginPDFPageWithInfo(CGRect, [AnyHashable : Any]?)

Marks the beginning of a new page in a PDF context and configures it using the specified custom values.

func UIGraphicsGetPDFContextBounds() -> CGRect

Returns the current page bounds.

func UIGraphicsAddPDFContextDestinationAtPoint(String, CGPoint)

Creates a jump destination in the current page.

func UIGraphicsSetPDFContextDestinationForRect(String, CGRect)

Links a rectangular area on the current page to the specified jump destination.

func UIGraphicsSetPDFContextURLForRect(URL, CGRect)

Links a rectangular area on the current page to the specified URL.

