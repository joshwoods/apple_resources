

- Core Graphics
-  CGPDFDictionaryApplyFunction(\_:\_:\_:) 

Function

# CGPDFDictionaryApplyFunction(\_:\_:\_:)

Applies a function to each entry in a dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFDictionaryApplyFunction(
    _ dict: CGPDFDictionaryRef,
    _ function: CGPDFDictionaryApplierFunction,
    _ info: UnsafeMutableRawPointer?
)
```

## Parameters 

`dict`  

A PDF dictionary. If this parameter is not a valid PDF dictionary, the behavior is undefined.

`function`  

The function to apply to each entry in the dictionary.

`info`  

A pointer to contextual information to pass to the function.

## Discussion

This function enumerates all of the entries in the dictionary, calling the function once for each. The current key, its associated value, and the contextual information are passed to the function (see also CGPDFDictionaryApplierFunction).

