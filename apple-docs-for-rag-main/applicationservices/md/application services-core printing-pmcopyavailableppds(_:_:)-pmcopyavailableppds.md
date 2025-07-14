

- Application Services
- Core Printing
-  PMCopyAvailablePPDs(\_:\_:) 

Function

# PMCopyAvailablePPDs(\_:\_:)

Obtains the list of PostScript printer description (PPD) files in a PPD domain.

macOS 10.3+

``` source
func PMCopyAvailablePPDs(
    _ domain: PMPPDDomain,
    _ ppds: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`domain`  

The PPD domain to search. See PMPPDDomain for a description of the constants you can use to specify the domain.

`ppds`  

A pointer to your CFArray variable. On return, the variable refers to a Core Foundation array of PPD files in the specified domain. Each element in the array is a Core Foundation URL object that specifies the location of a PPD file or a compressed PPD file. You are responsible for releasing the array. If the specified domain is not valid, the variable is set to `NULL`.

## Return Value

A result code. See Result Codes.

## See Also

### Accessing PostScript Printer Description Files

func PMCopyLocalizedPPD(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>) -> OSStatus

Obtains a localized PostScript printer description (PPD) file.

func PMCopyPPDData(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>) -> OSStatus

Obtains the uncompressed PPD data for a PostScript printer description (PPD) file.

