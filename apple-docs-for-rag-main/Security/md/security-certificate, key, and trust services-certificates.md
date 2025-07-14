

- Security
- Certificate, Key, and Trust Services
-  Certificates 

API Collection

# Certificates

Manage digital certificates.

## Overview

A digital certificate is a collection of data used to securely distribute the public half of a public/private key pair. Figure 1 shows the parts of a typical X.509 certificate that make this possible. Along with structural information, the certificate contains name and contact information for both its issuer and its owner (or subject), plus the owner’s public key. A date range indicates when the certificate is valid. Certificate extensions provide additional information and conditions, like acceptable uses for the public key. When assembling the certificate, to vouch for its integrity, the issuer digitally signs it using the issuer’s own identity (private key and certificate).

To evaluate a certificate, you first verify its signature using the specified algorithm and the issuer’s public key, which you obtain from the issuer’s publicly available certificate. A valid signature confirms that the certificate under evaluation, known as the leaf certificate, is unaltered. But in order to trust this result, you must also trust the issuer’s certificate. You use a similar procedure to test this certificate, and the one that guarantees that certificate, and the next, and so on in a chain back to a trusted root authority whose certificate, known as the anchor, which you trust implicitly. The public key included in the leaf certificate is then considered trustworthy. You can be assured that it has come unaltered from the certificate’s owner who controls the corresponding private key. This allows you to securely use the public key to engage in asymmetric cryptography with the certificate’s owner.

For more details about how certificates work, read Digital Certificates in Cryptographic Services Guide.

## Topics

### Essentials

Getting a Certificate

Obtain a certificate from an identity, from DER-encoded data, or from the keychain.

Storing a Certificate in the Keychain

Store a certificate in the keychain for safekeeping.

class SecCertificate

An abstract Core Foundation-type object representing an X.509 certificate.

func SecCertificateGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a certificate object belongs.

### Import and Export

Storing a DER-Encoded X.509 Certificate

Import and export a certificate from a file.

func SecCertificateCreateWithData(CFAllocator?, CFData) -> SecCertificate?

Creates a certificate object from a DER representation of a certificate.

func SecCertificateCopyData(SecCertificate) -> CFData

Returns a DER representation of a certificate given a certificate object.

### Certificate Components

Examining a Certificate

Learn how to retrieve properties from a certificate.

func SecCertificateCopySubjectSummary(SecCertificate) -> CFString?

Returns a human-readable summary of a certificate.

func SecCertificateCopyCommonName(SecCertificate, UnsafeMutablePointer&lt;CFString?>) -> OSStatus

Retrieves the common name of the subject of a certificate.

func SecCertificateCopyEmailAddresses(SecCertificate, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the email addresses for the subject of a certificate.

func SecCertificateCopyNormalizedIssuerSequence(SecCertificate) -> CFData?

Retrieves the normalized issuer sequence from a certificate.

func SecCertificateCopyNormalizedSubjectSequence(SecCertificate) -> CFData?

Retrieves the normalized subject sequence from a certificate.

func SecCertificateCopySerialNumberData(SecCertificate, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Returns the certificate’s serial number.

func SecCertificateCopyKey(SecCertificate) -> SecKey?

Retrieves the public key for a given certificate.

func SecCertificateCopyShortDescription(CFAllocator?, SecCertificate, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFString?

Returns a copy of the short description of a certificate.

func SecCertificateCopyLongDescription(CFAllocator?, SecCertificate, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFString?

Returns a copy of the long description of a certificate.

### Detailed Certificate Information

Getting Certificate Values

Obtain all the values associated with a certificate.

func SecCertificateCopyValues(SecCertificate, CFArray?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFDictionary?

Creates a dictionary that represents a certificate’s contents.

Certificate OIDs

Use OIDs as keys in the dictionary representing certificate values.

Certificate Property Keys

Recognize the dictionary keys that taken together define a certificate property.

Certificate Property Type Values

Recognize the possible certificate property types.

Certificate Item Attribute Constants

Use these four character values to indicate certificate item attributes.

### Certificate Names

func SecCertificateSetPreferred(SecCertificate?, CFString, CFArray?) -> OSStatus

Sets the certificate that should be preferred for the specified name and key use.

func SecCertificateCopyPreferred(CFString, CFArray?) -> SecCertificate?

Returns the preferred certificate for the specified name and key usage.

### Legacy Symbols

func SecCertificateAddToKeychain(SecCertificate, SecKeychain?) -> OSStatus

Adds a certificate to a keychain.

func SecCertificateCopyNormalizedIssuerContent(SecCertificate, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Returns a normalized copy of the distinguished name (DN) of the issuer of a certificate.

Deprecated

func SecCertificateCopyNormalizedSubjectContent(SecCertificate, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Returns a normalized copy of the distinguished name (DN) of the subject of a certificate.

Deprecated

func SecCertificateCopySerialNumber(SecCertificate) -> CFData?

Returns a copy of a certificate’s serial number.

Deprecated

func SecCertificateCopyPublicKey(SecCertificate) -> SecKey?

Retrieves the public key from a certificate.

Deprecated

