

- Core Graphics
-  CGPDFScannerPopArray(\_:\_:) 

Function

# CGPDFScannerPopArray(\_:\_:)

Retrieves an array object from the scanner stack.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFScannerPopArray(
    _ scanner: CGPDFScannerRef,
    _ value: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`scanner`  

A valid scanner object.

`value`  

On output, points to the PDF array object popped from the scanner stack.

## Return Value

true if the array object is retrieved successfully; otherwise, false.

## See Also

### Getting PDF Objects from the Scanner Stack

func CGPDFScannerPopObject(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFObjectRef?>?) -> Bool

Retrieves an object from the scanner stack.

func CGPDFScannerPopBoolean(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFBoolean>?) -> Bool

Retrieves a Boolean object from the scanner stack.

func CGPDFScannerPopInteger(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFInteger>?) -> Bool

Retrieves an integer object from the scanner stack.

func CGPDFScannerPopNumber(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFReal>?) -> Bool

Retrieves a real value object from the scanner stack.

func CGPDFScannerPopName(CGPDFScannerRef, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>?) -> Bool

Retrieves a character string from the scanner stack.

func CGPDFScannerPopString(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFStringRef?>?) -> Bool

Retrieves a string object from the scanner stack.

func CGPDFScannerPopDictionary(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFDictionaryRef?>?) -> Bool

Retrieves a PDF dictionary object from the scanner stack.

func CGPDFScannerPopStream(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFStreamRef?>?) -> Bool

Retrieves a PDF stream object from the scanner stack.

