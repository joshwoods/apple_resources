

- UIKit
-  UIGraphicsGetPDFContextBounds() 

Function

# UIGraphicsGetPDFContextBounds()

Returns the current page bounds.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func UIGraphicsGetPDFContextBounds() -> CGRect
```

## Return Value

The current page bounds associated with the PDF context or CGRectZero if the current context is not a PDF context.

## Discussion

If a page has not yet been started, this function returns the default media box you specified when you created the PDF context; otherwise, it returns the page bounds for the current page.

## See Also

### PDF creation

func UIGraphicsBeginPDFContextToData(NSMutableData, CGRect, [AnyHashable : Any]?)

Creates a PDF graphics context that targets the specified mutable data object.

func UIGraphicsBeginPDFContextToFile(String, CGRect, [AnyHashable : Any]?) -> Bool

Creates a PDF graphics context that targets a file at the specified path.

func UIGraphicsEndPDFContext()

Closes a PDF graphics context and pops it from the current context stack.

func UIGraphicsBeginPDFPage()

Marks the beginning of a new page in a PDF context and configures it using default values.

func UIGraphicsBeginPDFPageWithInfo(CGRect, [AnyHashable : Any]?)

Marks the beginning of a new page in a PDF context and configures it using the specified custom values.

func UIGraphicsAddPDFContextDestinationAtPoint(String, CGPoint)

Creates a jump destination in the current page.

func UIGraphicsSetPDFContextDestinationForRect(String, CGRect)

Links a rectangular area on the current page to the specified jump destination.

func UIGraphicsSetPDFContextURLForRect(URL, CGRect)

Links a rectangular area on the current page to the specified URL.

