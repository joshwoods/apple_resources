

- Core Graphics
-  CGPDFDictionaryApplierFunction 

Type Alias

# CGPDFDictionaryApplierFunction

Performs custom processing on a key-value pair from a PDF dictionary, using optional contextual information.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGPDFDictionaryApplierFunction = (UnsafePointer, CGPDFObjectRef, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`key`  

The current key in the dictionary.

`object`  

The value in the dictionary associated with the key.

`info`  

The contextual information that your provided in the `info` parameter in CGPDFDictionaryApplyFunction(_:_:_:).

## Discussion

CGPDFDictionaryApplierFunction defines the callback for CGPDFDictionaryApplyFunction(_:_:_:), that enumerates all of the entries in the dictionary, calling your custom applier function once for each entry. The current key, its associated value, and the contextual information are passed to your applier function using the `key`, `value`, and `info` parameters respectively.

