

- Core Graphics
-  CGPDFOperatorTableSetCallback(\_:\_:\_:) 

Function

# CGPDFOperatorTableSetCallback(\_:\_:\_:)

Sets a callback function for a PDF operator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFOperatorTableSetCallback(
    _ table: CGPDFOperatorTableRef,
    _ name: UnsafePointer,
    _ callback: CGPDFOperatorCallback
)
```

## Parameters 

`table`  

A PDF operator table.

`name`  

The name of the PDF operator you want to set a callback for.

`callback`  

The callback to invoke for the PDF operator specified by the `name` parameter.

## Discussion

You call the function CGPDFOperatorTableSetCallback(_:_:_:) for each PDF operator for which you want to provide a callback. See Appendix A in the *PDF Reference, Second Edition*, version 1.3, Adobe Systems Incorporated for a summary of PDF operators.

