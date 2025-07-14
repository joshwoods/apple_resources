

- Core Text
-  CTParagraphStyleGetValueForSpecifier(\_:\_:\_:\_:) 

Function

# CTParagraphStyleGetValueForSpecifier(\_:\_:\_:\_:)

Obtains the current value for a single setting specifier.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTParagraphStyleGetValueForSpecifier(
    _ paragraphStyle: CTParagraphStyle,
    _ spec: CTParagraphStyleSpecifier,
    _ valueBufferSize: Int,
    _ valueBuffer: UnsafeMutableRawPointer
) -> Bool
```

## Parameters 

`paragraphStyle`  

The paragraph style from which to get the value. This parameter may not be `NULL`.

`spec`  

The setting specifier for which to get the value.

`valueBufferSize`  

The size of the buffer pointed to by the `valueBuffer` parameter. This value must be at least as large as the size the required by the CTParagraphStyleSpecifier value set in the `spec` parameter.

`valueBuffer`  

On output, the requested setting value. The buffer’s size needs to be at least as large as the value passed into `valueBufferSize`. This parameter is required and may not be `NULL`.

## Return Value

`True` if `valueBuffer` was successfully filled; otherwise, `False`, indicating that one or more of the parameters are not valid.

## Discussion

This function returns the current value of the specifier whether or not the user actually set it. If the user did not set the specifier, this function returns the default value. If an invalid paragraph style setting specifier is passed into the `spec` parameter, nothing bad happens, and the buffer value is simply zeroed out. The reason is to allow backward compatibility with style setting specifiers that may be introduced in future versions.

