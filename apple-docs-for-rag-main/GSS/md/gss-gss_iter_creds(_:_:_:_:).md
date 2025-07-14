

- GSS
-  gss_iter_creds(\_:\_:\_:\_:) 

Function

# gss_iter_creds(\_:\_:\_:\_:)

Iterates over all credentials.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_iter_creds(
    _ min_stat: UnsafeMutablePointer,
    _ flags: OM_uint32,
    _ mech: gss_const_OID?,
    _ useriter: @escaping (gss_OID?, gss_cred_id_t?) -> Void
) -> OM_uint32
```

## Parameters 

`flags`  

No flags are currently defined. Pass 0 for this parameter.

`mech`  

The mechanism type of credentials to iterate over. Pass in `GSS_C_NO_OID_SET` to iterate over all credentials.

`useriter`  

A block that is called once for each credential. The block receives the credential’s mechanism and a copy of the credential as input on each iteration. Free the copy’s memory with a call to gss_release_cred(_:_:) when you are done with it. The block is called one final time with `NULL` inputs upon reaching the end of the list.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Discussion

Use the gss_iter_creds_f(_:_:_:_:_:) function if you want to track the callbacks using a user-supplied context.

## See Also

### Iteration

func gss_iter_creds_f(UnsafeMutablePointer&lt;OM_uint32>, OM_uint32, gss_const_OID?, UnsafeMutableRawPointer?, (UnsafeMutableRawPointer?, gss_OID?, gss_cred_id_t?) -> Void) -> OM_uint32

Iterates over all credentials with a user context.

