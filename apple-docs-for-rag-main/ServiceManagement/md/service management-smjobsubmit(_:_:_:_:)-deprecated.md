

- Service Management
-  SMJobSubmit(\_:\_:\_:\_:) Deprecated

Function

# SMJobSubmit(\_:\_:\_:\_:)

Submits the specified job to the specified domain.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.10Deprecated

**Mac Catalyst**

``` source
func SMJobSubmit(
    _ domain: CFString!,
    _ job: CFDictionary,
    _ auth: UnsafeMutableRawPointer!,
    _ outError: UnsafeMutablePointer?>!
) -> Bool
```

**macOS**

``` source
func SMJobSubmit(
    _ domain: CFString!,
    _ job: CFDictionary,
    _ auth: AuthorizationRef!,
    _ outError: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`domain`  

The job’s domain (for example, kSMDomainSystemLaunchd).

`job`  

A dictionary describing a job.

`auth`  

An `AuthorizationRef` containing the kSMRightModifySystemDaemons right if the specified

domain is kSMDomainSystemLaunchd.

`outError`  

An output reference to a `CFErrorRef` describing the specific error when submitting the job, or `NULL` if no error occurred. It’s the responsibility of the app to release the error reference. This argument can be `NULL`.

## Return Value

Returns true if the system successfully submits the job, otherwise `false`.

## See Also

### Deprecated Functions

func SMCopyAllJobDictionaries(CFString!) -> Unmanaged&lt;CFArray>!

Copies the job description dictionaries for all jobs in the specified domain.

Deprecated

func SMJobCopyDictionary(CFString!, CFString) -> Unmanaged&lt;CFDictionary>!

Copies the job description dictionary for the specified job label.

Deprecated

func SMJobRemove(CFString!, CFString, UnsafeMutableRawPointer!, Bool, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes the job with the specified label from the specified domain.

Deprecated

