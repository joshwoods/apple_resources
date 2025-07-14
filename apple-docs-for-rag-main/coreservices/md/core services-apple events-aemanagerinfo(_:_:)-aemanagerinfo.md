

- Core Services
- Apple Events
-  AEManagerInfo(\_:\_:) 

Function

# AEManagerInfo(\_:\_:)

Provides information about the version of the Apple Event Manager currently available or the number of processes that are currently recording Apple events.

macOS 10.0+

``` source
func AEManagerInfo(
    _ keyWord: AEKeyword,
    _ result: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`keyWord`  

A value that determines the kind of information the function supplies in the `result` parameter.

Pass the value `keyAERecorderCount` to obtain the number of processes that are currently recording Apple events.

Pass the value `keyAEVersion` to obtain version information for the Apple Event Manager, in `NumVersion` format.

Some keyword constants are defined in Keyword Parameter Constants.

See AEKeyword.

`result`  

A pointer to a long value. On return, provides information that depends on what you pass in the `keyword` parameter.

If you pass `keyAERecorderCount`, `result` specifies the number of processes that are currently recording Apple events.

If you pass `keyAEVersion`, `result` supplies version information for the Apple Event Manager, in a format that matches the `'vers'` resource.

## Return Value

A result code. See Result Codes.

## Discussion

For recordable applications, the information provided by `AEManagerInfo` may be useful when the application is responding to Apple events that it sends to itself.

For information on determining whether the Apple Event Manager is available, see the Apple Event Manager Gestalt Selector, described in *Inside macOS: Gestalt Manager Reference*.

### Version-Notes

Thread safe starting in OS X v10.2.

The `AEManagerInfo` function is available only in version 1.01 and later of the Apple Event Manager.

