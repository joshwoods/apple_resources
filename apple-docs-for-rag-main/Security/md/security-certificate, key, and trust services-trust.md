

- Security
- Certificate, Key, and Trust Services
-  Trust 

API Collection

# Trust

Evaluate trust based on a given policy.

## Overview

Before using a certificate, you evaluate its trustworthiness for a particular purpose.

If you know that a certificate comes unaltered from its sender, you can be confident that its embedded public key does as well. You can also take at face value claims made by the certificate about when and for what purpose the public key may be used. You can securely engage in the operations described in Using Keys for Encryption and Signing and Verifying without prior arrangement between sender and receiver.

## Topics

### Essentials

Creating a Trust Object

Construct a trust object from a certificate and a policy.

func SecTrustCreateWithCertificates(CFTypeRef, CFTypeRef?, UnsafeMutablePointer&lt;SecTrust?>) -> OSStatus

Creates a trust management object based on certificates and policies.

class SecTrust

An object used to evaluate trust.

func SecTrustGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a trust object belongs.

### Trust Evaluation

Evaluating a Trust and Parsing the Result

Learn what to expect when evaluating a trust object.

func SecTrustEvaluateWithError(SecTrust, UnsafeMutablePointer&lt;CFError?>?) -> Bool

Evaluates trust for the specified certificate and policies.

func SecTrustEvaluateAsyncWithError(SecTrust, dispatch_queue_t, SecTrustWithErrorCallback) -> OSStatus

Evaluates a trust object asynchronously on the specified dispatch queue.

typealias SecTrustWithErrorCallback

A block called with the results of an asynchronous trust evaluation.

### Trust Evaluation Result

Discovering Why a Trust Evaluation Failed

Determine whether you can recover from a failed trust evaluation.

func SecTrustGetTrustResult(SecTrust, UnsafeMutablePointer&lt;SecTrustResultType>) -> OSStatus

Returns the result code from the most recent trust evaluation.

enum SecTrustResultType

Trust evaluation result codes.

func SecTrustCopyResult(SecTrust) -> CFDictionary?

Returns a dictionary containing information about an evaluated trust.

Trust Result Dictionary Keys

Recognize the keys that appear in a dictionary containing information about an evaluated certification chain.

### Trust Components

func SecTrustCopyPublicKey(SecTrust) -> SecKey?

Returns the public key for a leaf certificate after it has been evaluated.

Deprecated

func SecTrustGetCertificateCount(SecTrust) -> CFIndex

Returns the number of certificates in an evaluated certificate chain.

func SecTrustGetCertificateAtIndex(SecTrust, CFIndex) -> SecCertificate?

Returns a specific certificate from the certificate chain used to evaluate trust.

Deprecated

func SecTrustGetVerifyTime(SecTrust) -> CFAbsoluteTime

Gets the absolute time against which the certificates in a trust management object are verified.

func SecTrustCopyAnchorCertificates(UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the anchor (root) certificates stored by macOS.

func SecTrustCopyCustomAnchorCertificates(SecTrust, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the custom anchor certificates, if any, used by a given trust.

func SecTrustCopyExceptions(SecTrust) -> CFData?

Returns an opaque cookie containing exceptions to trust policies that will allow future evaluations of the current certificate to succeed.

func SecTrustCopyPolicies(SecTrust, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the policies used by a given trust management object.

func SecTrustCopyProperties(SecTrust) -> CFArray?

Returns an array containing the properties of a trust object.

Deprecated

### Advanced Trust Configuation

Configuring a Trust

Work around a recoverable trust failure.

func SecTrustSetVerifyDate(SecTrust, CFDate) -> OSStatus

Sets the date and time against which the certificates in a trust management object are verified.

func SecTrustSetAnchorCertificates(SecTrust, CFArray?) -> OSStatus

Sets the anchor certificates used when evaluating a trust management object.

func SecTrustSetAnchorCertificatesOnly(SecTrust, Bool) -> OSStatus

Reenables trusting built-in anchor certificates.

func SecTrustSetExceptions(SecTrust, CFData?) -> Bool

Sets a list of exceptions that should be ignored when the certificate is evaluated.

func SecTrustSetPolicies(SecTrust, CFTypeRef) -> OSStatus

Sets the policies to use in an evaluation.

func SecTrustSetOptions(SecTrust, SecTrustOptionFlags) -> OSStatus

Sets option flags for customizing evaluation of a trust object.

struct SecTrustOptionFlags

The option flags used to condition a trust evaluation.

func SecTrustGetNetworkFetchAllowed(SecTrust, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether a trust evaluation is permitted to fetch missing intermediate certificates from the network.

func SecTrustSetNetworkFetchAllowed(SecTrust, Bool) -> OSStatus

Specifies whether a trust evaluation is permitted to fetch missing intermediate certificates from the network.

func SecTrustSetOCSPResponse(SecTrust, CFTypeRef?) -> OSStatus

Attaches Online Certificate Status Protocol (OSCP) response data to a trust object.

func SecTrustSetSignedCertificateTimestamps(SecTrust, CFArray?) -> OSStatus

Attaches signed certificate timestamp data to a trust object.

### Trust Settings

func SecTrustSettingsCopyCertificates(SecTrustSettingsDomain, UnsafeMutablePointer&lt;CFArray?>?) -> OSStatus

Obtains an array of all certificates that have trust settings in a specific trust settings domain.

func SecTrustSettingsCopyModificationDate(SecCertificate, SecTrustSettingsDomain, UnsafeMutablePointer&lt;CFDate?>) -> OSStatus

Obtains the date and time at which a certificate’s trust settings were last modified.

Usage Constraints Dictionary Keys

Use these trust settings keys in a usage constraints dictionary.

func SecTrustSettingsCopyTrustSettings(SecCertificate, SecTrustSettingsDomain, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Obtains the trust settings for a certificate.

func SecTrustSettingsCreateExternalRepresentation(SecTrustSettingsDomain, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Obtains an external, portable representation of the specified domain’s trust settings.

func SecTrustSettingsImportExternalRepresentation(SecTrustSettingsDomain, CFData) -> OSStatus

Imports trust settings into a trust domain.

func SecTrustSettingsRemoveTrustSettings(SecCertificate, SecTrustSettingsDomain) -> OSStatus

Deletes the trust settings for a certificate.

func SecTrustSettingsSetTrustSettings(SecCertificate, SecTrustSettingsDomain, CFTypeRef?) -> OSStatus

Specifies trust settings for a certificate.

struct SecTrustSettingsKeyUsage

Allowed uses for the encryption key in a certificate.

enum SecTrustSettingsResult

Trust settings returned in usage constraints dictionaries.

enum SecTrustSettingsDomain

The trust settings domains.

### Legacy Symbols

func SecTrustEvaluate(SecTrust, UnsafeMutablePointer&lt;SecTrustResultType>) -> OSStatus

Evaluates trust for the specified certificate and policies.

Deprecated

func SecTrustEvaluateAsync(SecTrust, dispatch_queue_t?, SecTrustCallback) -> OSStatus

Evaluates a trust object asynchronously on the specified dispatch queue.

Deprecated

typealias SecTrustCallback

A block called with the results of an asynchronous trust evaluation.

func SecTrustSetKeychains(SecTrust, CFTypeRef?) -> OSStatus

Sets the keychains searched for intermediate certificates when evaluating a trust management object.

Deprecated

