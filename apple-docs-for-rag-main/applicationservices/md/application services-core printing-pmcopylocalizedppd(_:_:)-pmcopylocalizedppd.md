

- Application Services
- Core Printing
-  PMCopyLocalizedPPD(\_:\_:) 

Function

# PMCopyLocalizedPPD(\_:\_:)

Obtains a localized PostScript printer description (PPD) file.

macOS 10.3+

``` source
func PMCopyLocalizedPPD(
    _ ppd: CFURL,
    _ localizedPPD: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`ppd`  

A Core Foundation URL object for a PPD file. You can obtain a PPD URL using the function PMCopyAvailablePPDs(_:_:).

`localizedPPD`  

A pointer to your CFURL variable. On return, the variable refers to a Core Foundation URL object. The URL specifies the location of a PPD file or a compressed PPD file that has been localized for the current user's language preference. You are responsible for releasing the URL. If the `ppd` parameter is not valid, the variable is set to `NULL`.

## Return Value

A result code. See Result Codes.

## Discussion

To access the data in the PPD file, you can use the function PMCopyPPDData(_:_:).

### Special Considerations

In macOS 10.5 and later, the printing system supports globalized PPD files as defined in CUPS version 1.2 and later. A globalized PPD file contains multiple localizations within a single file. If a globalized PPD file exists, this function returns the URL to this file and it is up to the application to obtain the correct localized data. For more information, see CUPS PPD Extensions.

## See Also

### Accessing PostScript Printer Description Files

func PMCopyAvailablePPDs(PMPPDDomain, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

Obtains the list of PostScript printer description (PPD) files in a PPD domain.

func PMCopyPPDData(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>) -> OSStatus

Obtains the uncompressed PPD data for a PostScript printer description (PPD) file.

