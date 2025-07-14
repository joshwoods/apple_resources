

- Application Services
- Core Printing
-  PMCopyPPDData(\_:\_:) 

Function

# PMCopyPPDData(\_:\_:)

Obtains the uncompressed PPD data for a PostScript printer description (PPD) file.

macOS 10.3+

``` source
func PMCopyPPDData(
    _ ppd: CFURL,
    _ data: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`ppd`  

A URL for a PPD or compressed PPD file. You can obtain a PPD URL using the function PMCopyAvailablePPDs(_:_:) or PMCopyLocalizedPPD(_:_:).

`data`  

A pointer to your CFData variable. On return, the variable refers to a Core Foundation data object containing the uncompressed PPD data from the specified PPD file. You are responsible for releasing the data object. If the `ppd` parameter does not reference a PPD file, the variable is set to `NULL`.

## Return Value

A result code. See Result Codes.

## See Also

### Accessing PostScript Printer Description Files

func PMCopyAvailablePPDs(PMPPDDomain, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains the list of PostScript printer description (PPD) files in a PPD domain.

func PMCopyLocalizedPPD(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>) -> OSStatus

Obtains a localized PostScript printer description (PPD) file.

