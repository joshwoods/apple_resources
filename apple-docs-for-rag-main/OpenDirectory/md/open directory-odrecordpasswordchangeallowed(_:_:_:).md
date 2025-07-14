

- Open Directory
-  ODRecordPasswordChangeAllowed(\_:\_:\_:) 

Function

# ODRecordPasswordChangeAllowed(\_:\_:\_:)

Mac CatalystmacOS 10.10+

``` source
func ODRecordPasswordChangeAllowed(
    _ record: ODRecordRef!,
    _ newPassword: CFString!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

## See Also

### Functions

func ODNodeAddAccountPolicy(ODNodeRef!, CFDictionary!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeCopyAccountPolicies(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFDictionary!

func ODNodeCopyPolicies(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

func ODNodeCopySupportedPolicies(ODNodeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

func ODNodeCustomFunction(ODNodeRef!, CFString!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFTypeRef!

func ODNodePasswordContentCheck(ODNodeRef!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeRemoveAccountPolicy(ODNodeRef!, CFDictionary!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeRemovePolicy(ODNodeRef!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeSetAccountPolicies(ODNodeRef!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeSetPolicies(ODNodeRef!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODNodeSetPolicy(ODNodeRef!, String!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordAddAccountPolicy(ODRecordRef!, CFDictionary!, String!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordAuthenticationAllowed(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

func ODRecordCopyAccountPolicies(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFDictionary!

func ODRecordCopyEffectivePolicies(ODRecordRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

