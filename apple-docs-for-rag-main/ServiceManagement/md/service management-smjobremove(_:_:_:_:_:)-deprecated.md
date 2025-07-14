

- Service Management
-  SMJobRemove(\_:\_:\_:\_:\_:) Deprecated

Function

# SMJobRemove(\_:\_:\_:\_:\_:)

Removes the job with the specified label from the specified domain.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.10Deprecated

**Mac Catalyst**

``` source
func SMJobRemove(
    _ domain: CFString!,
    _ jobLabel: CFString,
    _ auth: UnsafeMutableRawPointer!,
    _ wait: Bool,
    _ outError: UnsafeMutablePointer?>!
) -> Bool
```

**macOS**

``` source
func SMJobRemove(
    _ domain: CFString!,
    _ jobLabel: CFString,
    _ auth: AuthorizationRef!,
    _ wait: Bool,
    _ outError: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`domain`  

The job’s domain (for example, kSMDomainSystemLaunchd).

`jobLabel`  

The label identifier of the job to remove.

`auth`  

An `AuthorizationRef` containing the kSMRightModifySystemDaemons right if the specified domain is kSMDomainSystemLaunchd.

`wait`  

Pass `true` to block until the process for the specified job has exited.

`outError`  

An output reference to a `CFErrorRef` describing the specific error when removing the job, or `NULL` if no error occurred. It’s the responsibility of the app to release the error reference. This argument can be `NULL`.

## Return Value

Returns `true` if the system successfully removes the job, otherwise `false`.

## Discussion

If the job is currently running, it conditionally blocks until the running process has exited.

## See Also

### Deprecated Functions

func SMCopyAllJobDictionaries(CFString!) -> Unmanaged&lt;CFArray>!

Copies the job description dictionaries for all jobs in the specified domain.

Deprecated

func SMJobCopyDictionary(CFString!, CFString) -> Unmanaged&lt;CFDictionary>!

Copies the job description dictionary for the specified job label.

Deprecated

func SMJobSubmit(CFString!, CFDictionary, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Submits the specified job to the specified domain.

Deprecated

