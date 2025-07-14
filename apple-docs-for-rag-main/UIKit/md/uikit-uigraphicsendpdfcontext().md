

- UIKit
-  UIGraphicsEndPDFContext() 

Function

# UIGraphicsEndPDFContext()

Closes a PDF graphics context and pops it from the current context stack.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func UIGraphicsEndPDFContext()
```

## Discussion

You must call this function after you finish drawing to a PDF graphics context. This function closes the current open page and removes the PDF context from the graphics context stack. It also releases the CGContext associated with the PDF context. If the current graphics context is not a PDF context, this function does nothing.

## See Also

### PDF creation

func UIGraphicsBeginPDFContextToData(NSMutableData, CGRect, [AnyHashable : Any]?)

Creates a PDF graphics context that targets the specified mutable data object.

func UIGraphicsBeginPDFContextToFile(String, CGRect, [AnyHashable : Any]?) -> Bool

Creates a PDF graphics context that targets a file at the specified path.

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

