

- Service Management
-  SMJobCopyDictionary(\_:\_:) Deprecated

Function

# SMJobCopyDictionary(\_:\_:)

Copies the job description dictionary for the specified job label.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.10Deprecated

``` source
func SMJobCopyDictionary(
    _ domain: CFString!,
    _ jobLabel: CFString
) -> Unmanaged!
```

## Parameters 

`domain`  

The job’s domain (for example, kSMDomainSystemLaunchd).

`jobLabel`  

The label identifier of the job to copy.

## Return Value

A new dictionary describing the job, or `NULL` if the system couldn’t find the job. The caller must release the dictionary.

## See Also

### Deprecated Functions

func SMCopyAllJobDictionaries(CFString!) -> Unmanaged&lt;CFArray>!

Copies the job description dictionaries for all jobs in the specified domain.

Deprecated

func SMJobRemove(CFString!, CFString, UnsafeMutableRawPointer!, Bool, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes the job with the specified label from the specified domain.

Deprecated

func SMJobSubmit(CFString!, CFDictionary, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Submits the specified job to the specified domain.

Deprecated

