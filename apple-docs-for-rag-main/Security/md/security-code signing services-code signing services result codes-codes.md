

- Security
- Code Signing Services
-  Code Signing Services Result Codes 

API Collection

# Code Signing Services Result Codes

Recognize result codes specific to the code signing services API.

## Discussion

Use the SecCopyErrorMessageString(_:_:) function to obtain a human readable string corresponding to these status codes.

The functions of the Code Signing Services API may also return the general codes listed in Security Framework Result Codes. In particular, you might expect to encounter errSecSuccess, errSecUnimplemented, errSecParam, and errSecAllocate.

## Topics

### Code-signing format result codes

var errSecCSAmbiguousBundleFormat: OSStatus

The bundle could be an app or a framework.

var errSecCSBadBundleFormat: OSStatus

The bundle format is unrecognized, invalid, or unsuitable.

var errSecCSBadDictionaryFormat: OSStatus

A required information property list (Info.plist) file or resource is malformed.

var errSecCSBadDiskImageFormat: OSStatus

The disk image format unrecognized, invalid, or unsuitable.

var errSecCSBadObjectFormat: OSStatus

The object file format invalid or unsuitable.

### Code-signing database issue result codes

var errSecCSDBAccess: OSStatus

Cannot access signature database.

var errSecCSDBDenied: OSStatus

Access to signature database denied.

var errSecCSDbCorrupt: OSStatus

A system database or file is corrupt.

var errSecCSSigDBAccess: OSStatus

Can’t access signature database.

var errSecCSSigDBDenied: OSStatus

Access to signature database denied.

### Code-signing host protocol issue result codes

var errSecCSHostProtocolContradiction: OSStatus

Host protocol violation: contradictory hosting modes.

var errSecCSHostProtocolDedicationError: OSStatus

Host protocol violation: operation not allowed with or for a dedicated guest.

var errSecCSHostProtocolInvalidAttribute: OSStatus

Code signing host returned invalid or inconsistent attributes for guest code.

var errSecCSHostProtocolInvalidHash: OSStatus

Host protocol violation: invalid hash of guest code.

var errSecCSHostProtocolNotProxy: OSStatus

Host protocol violation: proxy hosting not engaged.

var errSecCSHostProtocolRelativePath: OSStatus

Host protocol violation: absolute guest path required.

var errSecCSHostProtocolStateError: OSStatus

Host protocol violation: invalid guest state change request.

var errSecCSHostProtocolUnrelated: OSStatus

Host protocol violation: the specified code is not a guest of the specified code signing host.

### Code-signing signature issue result codes

var errSecCSSignatureFailed: OSStatus

Code or signature modified.

var errSecCSSignatureInvalid: OSStatus

Invalid format for signature.

var errSecCSSignatureNotVerifiable: OSStatus

Signature cannot be read.

var errSecCSSignatureUnsupported: OSStatus

Unsupported type or version of signature.

var errSecCSUnsigned: OSStatus

Code object is not signed.

var errSecCSUnsignedNestedCode: OSStatus

Nested code is unsigned.

var errSecCSUnsupportedDigestAlgorithm: OSStatus

The signature digest algorithm(s) specified are not supported.

var errSecCSSignatureUntrusted: OSStatus

The signature is valid but signer isn’t trusted.

### Code-signing file format issue result codes

var errSecCSDSStoreSymlink: OSStatus

A `.DS_Store` file can’t be a symlink.

var errSecCSFileHardQuarantined: OSStatus

File open or execution not allowed.

var errSecCSInvalidSymlink: OSStatus

Invalid destination for symbolic link in bundle.

var errSecCSNoMainExecutable: OSStatus

The code has no main executable file.

var errSecCSRegularFile: OSStatus

The main executable or Info.plist must be a regular file (and not, for example, a symbolic link).

var errSecCSUnsealedAppRoot: OSStatus

Unsealed contents present in the bundle root.

var errSecCSUnsealedFrameworkRoot: OSStatus

Unsealed contents present in the root directory of an embedded framework.

### Code-signing resource issue result codes

var errSecCSResourceDirectoryFailed: OSStatus

A directory or its signature has been modified and is therefore invalid.

var errSecCSResourceNotSupported: OSStatus

Found an unsupported resource.

var errSecCSResourceRulesInvalid: OSStatus

Invalid resource selection rule or rules.

var errSecCSResourcesInvalid: OSStatus

The sealed resource directory is invalid.

var errSecCSResourcesNotFound: OSStatus

Cannot find sealed resources in code.

var errSecCSResourcesNotSealed: OSStatus

Resources are not sealed by the signature.

### Other result codes

var errSecCSBadCallbackValue: OSStatus

The monitor callback returned invalid value.

var errSecCSBadFrameworkVersion: OSStatus

The embedded framework contains a modified or invalid version.

var errSecCSBadLVArch: OSStatus

The library validation flag cannot be used with an i386 binary.

var errSecCSBadMainExecutable: OSStatus

The main executable failed strict validation.

var errSecCSBadNestedCode: OSStatus

The nested code is modified or invalid.

var errSecCSBadResource: OSStatus

A sealed resource is missing or invalid.

var errSecCSCMSTooLarge: OSStatus

The signature is too large to embed.

var errSecCSCancelled: OSStatus

The operation was terminated by explicit cancellation.

var errSecCSGuestInvalid: OSStatus

The identity of guest code has been invalidated.

var errSecCSHelperFailed: OSStatus

The codesign_allocate helper tool can’t be found or used.

var errSecCSHostReject: OSStatus

Code rejected its host.

var errSecCSInfoPlistFailed: OSStatus

The Info.plist file or the signature has been modified.

var errSecCSInternalError: OSStatus

Internal error in Code Signing Services subsystem.

var errSecCSInvalidAttributeValues: OSStatus

An attribute value associated with a key is out of range or is the wrong type.

var errSecCSInvalidFlags: OSStatus

Invalid or inappropriate API flags specified.

var errSecCSInvalidObjectRef: OSStatus

Invalid API object reference.

var errSecCSInvalidPlatform: OSStatus

Invalid platform identifier or platform mismatch.

var errSecCSMultipleGuests: OSStatus

Code signing host has more than one block of guest code with this attribute value.

var errSecCSNoMatches: OSStatus

No matches were found for a search or update operation.

var errSecCSNoSuchCode: OSStatus

Code signing host has no guest code with the requested attributes.

var errSecCSNotAHost: OSStatus

This code is not a code signing host.

var errSecCSNotAppLike: OSStatus

The code is valid but does not seem to be an app.

var errSecCSNotSupported: OSStatus

Operation not supported for this type of code.

var errSecCSObjectRequired: OSStatus

A required pointer argument was null.

var errSecCSOutdated: OSStatus

The presented data is out of date.

var errSecCSReqFailed: OSStatus

The code failed to satisfy one of the code requirements.

var errSecCSReqInvalid: OSStatus

Invalid or corrupted code requirements.

var errSecCSReqUnsupported: OSStatus

Unsupported type or version of code requirements.

var errSecCSStaticCodeChanged: OSStatus

The code on disk has been modified after the code started running.

var errSecCSStaticCodeNotFound: OSStatus

Cannot find code object on disk.

var errSecCSTooBig: OSStatus

The code is too big for current signing format.

var errSecCSUnimplemented: OSStatus

Unimplemented code signing feature.

var errSecCSUnsupportedGuestAttributes: OSStatus

Cannot locate guest code using this attribute set.

var errSecCSVetoed: OSStatus

var errSecCSWeakResourceEnvelope: OSStatus

The resource envelope is obsolete (version 1 signature).

var errSecCSWeakResourceRules: OSStatus

The resource envelope is obsolete (custom omit rules).

var errSecCSBadTeamIdentifier: OSStatus

A Team Identifier is wrong or inappropriate.

var errSecCSInvalidAssociatedFileData: OSStatus

Resource fork, Finder information, or similar detritus not allowed.

var errSecCSInvalidTeamIdentifier: OSStatus

A Team Identifier string is invalid.

var errSecMultipleExecSegments: OSStatus

The image contains multiple executable segments.

var errSecCSInvalidEntitlements: OSStatus

Encountered an invalid entitlement plist.

var errSecCSInvalidRuntimeVersion: OSStatus

An invalid runtime version was explicity set.

var errSecCSRevokedNotarization: OSStatus

Notarization indicates this code has been revoked.

