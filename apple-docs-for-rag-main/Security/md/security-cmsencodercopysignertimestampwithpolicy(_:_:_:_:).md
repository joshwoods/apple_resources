

- Security
-  CMSEncoderCopySignerTimestampWithPolicy(\_:\_:\_:\_:) 

Function

# CMSEncoderCopySignerTimestampWithPolicy(\_:\_:\_:\_:)

Returns the timestamp of a signer of a CMS message using a particular policy, if present.

macOS 10.10+

``` source
func CMSEncoderCopySignerTimestampWithPolicy(
    _ cmsEncoder: CMSEncoder,
    _ timeStampPolicy: CFTypeRef?,
    _ signerIndex: Int,
    _ timestamp: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

A CMSEncoder reference returned by the CMSEncoderCreate(_:) function.

`timeStampPolicy`  

A timestamp policy. Specify `NULL` (or use the CMSEncoderCopySignerTimestamp(_:_:_:) function instead) to get the default, which is a policy using kSecPolicyAppleTimeStamping. See Policies in Certificate, Key, and Trust Services for more about policies.

`signerIndex`  

A number indicating which signer to examine. Signer index numbers start with 0. Use the CMSDecoderGetNumSigners(_:_:) function to determine the total number of signers for a message.

`timestamp`  

The address of an absolute time value where the result should be stored.

## Return Value

A result code. See Security Framework Result Codes.

