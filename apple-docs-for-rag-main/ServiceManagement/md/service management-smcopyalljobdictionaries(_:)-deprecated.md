

- Service Management
-  SMCopyAllJobDictionaries(\_:) Deprecated

Function

# SMCopyAllJobDictionaries(\_:)

Copies the job description dictionaries for all jobs in the specified domain.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.10Deprecated

``` source
func SMCopyAllJobDictionaries(_ domain: CFString!) -> Unmanaged!
```

## Parameters 

`domain`  

The job’s domain (for example, kSMDomainSystemLaunchd).

## Return Value

A new array containing all job dictionaries, or `NULL` if an error occurred. The caller must release the array.

## See Also

### Deprecated Functions

func SMJobCopyDictionary(CFString!, CFString) -> Unmanaged&lt;CFDictionary>!

Copies the job description dictionary for the specified job label.

Deprecated

func SMJobRemove(CFString!, CFString, UnsafeMutableRawPointer!, Bool, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes the job with the specified label from the specified domain.

Deprecated

func SMJobSubmit(CFString!, CFDictionary, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Submits the specified job to the specified domain.

Deprecated

