

- UIKit
-  UIGraphicsBeginPDFPage() 

Function

# UIGraphicsBeginPDFPage()

Marks the beginning of a new page in a PDF context and configures it using default values.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func UIGraphicsBeginPDFPage()
```

## Discussion

This function ends any previous page before beginning a new one. It sets the media box of the new page to the rectangle you specified when you created the PDF context.

If the current graphics context is not a PDF context, this function does nothing.

You must call this function or the UIGraphicsBeginPDFPageWithInfo(_:_:) function before you issue any drawing commands.

## See Also

### PDF creation

func UIGraphicsBeginPDFContextToData(NSMutableData, CGRect, [AnyHashable : Any]?)

Creates a PDF graphics context that targets the specified mutable data object.

func UIGraphicsBeginPDFContextToFile(String, CGRect, [AnyHashable : Any]?) -> Bool

Creates a PDF graphics context that targets a file at the specified path.

func UIGraphicsEndPDFContext()

Closes a PDF graphics context and pops it from the current context stack.

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

