

- Security
-  Cryptographic Message Syntax Services 

API Collection

# Cryptographic Message Syntax Services

Cryptographically sign and encrypt S/MIME messages.

## Overview

When you want to exchange data securely using the Multipurpose Internet Mail Extensions (MIME) protocol, you use the version of the protocol known as S/MIME defined in RFC 3851. This allows you to, among other things, ensure data integrity through digital signatures and data confidentiality through encryption. S/MIME in turn relies on the Cryptographic Message Syntax (CMS) protocol defined in RFC 3852 to carry out these operations.

Cryptographic message syntax services provides encoder objects that perform encryption using the CMS protocol’s enveloped-data content type and sign using the signed-data content type. When a message is both signed and encrypted, the enveloped data content contains the signed data content. That is, the message is first signed and then the signed content is encrypted.

## Topics

### The Encoder

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

class CMSEncoder

Opaque reference to a CMS encoder object.

func CMSEncoderGetTypeID() -> CFTypeID

Returns the type identifier for the CMSEncoder opaque type.

### Message Creation

func CMSEncoderAddSigners(CMSEncoder, CFTypeRef) -> OSStatus

Specifies signers of the message.

func CMSEncoderAddRecipients(CMSEncoder, CFTypeRef) -> OSStatus

Specifies a message is to be encrypted and specifies the recipients of the message.

func CMSEncoderSetHasDetachedContent(CMSEncoder, Bool) -> OSStatus

Specifies whether the signed data is to be separate from the message.

func CMSEncoderSetEncapsulatedContentTypeOID(CMSEncoder, CFTypeRef) -> OSStatus

Specifies an object identifier for the encapsulated data of a signed message.

func CMSEncoderAddSupportingCerts(CMSEncoder, CFTypeRef) -> OSStatus

Adds certificates to a message.

func CMSEncoderAddSignedAttributes(CMSEncoder, CMSSignedAttributes) -> OSStatus

Specifies attributes for a signed message.

struct CMSSignedAttributes

Optional attributes you can add to a signed message.

func CMSEncoderSetCertificateChainMode(CMSEncoder, CMSCertificateChainMode) -> OSStatus

Specifies which certificates to include in a signed CMS message.

enum CMSCertificateChainMode

Constants that can be set to specify what certificates to include in a signed message.

func CMSEncoderSetSignerAlgorithm(CMSEncoder, CFString) -> OSStatus

Sets the digest algorithm to use for the signer.

### Message Characteristics

func CMSEncoderCopySigners(CMSEncoder, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Obtains the array of signers specified with the `CMSEncoderAddSigners` function.

func CMSEncoderCopyRecipients(CMSEncoder, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Obtains the array of recipients specified with the `CMSEncoderAddRecipients` function.

func CMSEncoderGetHasDetachedContent(CMSEncoder, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether the message is to have detached content.

func CMSEncoderCopyEncapsulatedContentType(CMSEncoder, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Obtains the object identifier for the encapsulated data of a signed message.

func CMSEncoderCopySupportingCerts(CMSEncoder, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Obtains the certificates added to a message with `CMSEncoderAddSupportingCerts`.

func CMSEncoderGetCertificateChainMode(CMSEncoder, UnsafeMutablePointer&lt;CMSCertificateChainMode>) -> OSStatus

Obtains a constant that indicates which certificates are to be included in a signed CMS message.

### Encoding

func CMSEncoderUpdateContent(CMSEncoder, UnsafeRawPointer, Int) -> OSStatus

Feeds content bytes into the encoder.

func CMSEncoderCopyEncodedContent(CMSEncoder, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Finishes encoding the message and obtains the encoded result.

func CMSEncodeContent(CFTypeRef?, CFTypeRef?, CFTypeRef?, Bool, CMSSignedAttributes, UnsafeRawPointer, Int, UnsafeMutablePointer&lt;CFData?>?) -> OSStatus

Encodes a message and obtains the result in one high-level function call.

### The Decoder

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

class CMSDecoder

An opaque reference to a CMS decoder object.

func CMSDecoderGetTypeID() -> CFTypeID

Returns the type identifier for the CMSDecoder opaque type.

### Decoding

func CMSDecoderUpdateMessage(CMSDecoder, UnsafeRawPointer, Int) -> OSStatus

Feeds raw bytes of the message to be decoded into the decoder.

func CMSDecoderFinalizeMessage(CMSDecoder) -> OSStatus

Indicates that there is no more data to decode.

func CMSDecoderSetDetachedContent(CMSDecoder, CFData) -> OSStatus

Specifies the message’s detached content, if any.

func CMSDecoderCopyDetachedContent(CMSDecoder, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Obtains the detached content specified with the `CMSDecoderSetDetachedContent` function.

### Signature Verification

func CMSDecoderSetSearchKeychain(CMSDecoder, CFTypeRef) -> OSStatus

Specifies the keychains to search for intermediate certificates to be used in verifying a signed message’s signer certificates.

Deprecated

func CMSDecoderGetNumSigners(CMSDecoder, UnsafeMutablePointer&lt;Int>) -> OSStatus

Obtains the number of signers of a message.

func CMSDecoderCopySignerEmailAddress(CMSDecoder, Int, UnsafeMutablePointer&lt;CFString?>) -> OSStatus

Obtains the email address of the specified signer of a CMS message.

func CMSDecoderCopySignerCert(CMSDecoder, Int, UnsafeMutablePointer&lt;SecCertificate?>) -> OSStatus

Obtains the certificate of the specified signer of a CMS message.

func CMSDecoderCopySignerStatus(CMSDecoder, Int, CFTypeRef, Bool, UnsafeMutablePointer&lt;CMSSignerStatus>?, UnsafeMutablePointer&lt;SecTrust?>?, UnsafeMutablePointer&lt;OSStatus>?) -> OSStatus

Obtains the status of a CMS message’s signature.

enum CMSSignerStatus

The constants that indicate the status of the signature and signer information in a signed message.

### Message Content

func CMSDecoderIsContentEncrypted(CMSDecoder, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Determines whether a CMS message was encrypted.

func CMSDecoderCopyEncapsulatedContentType(CMSDecoder, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Obtains the object identifier for the encapsulated data of a signed message.

func CMSDecoderCopyAllCerts(CMSDecoder, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Obtains an array of all of the certificates in a message.

func CMSDecoderCopyContent(CMSDecoder, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Obtains the message content, if any.

### Timestamps

func CMSDecoderCopySignerSigningTime(CMSDecoder, Int, UnsafeMutablePointer&lt;CFAbsoluteTime>) -> OSStatus

Obtains the signing time of a CMS message, if present.

func CMSDecoderCopySignerTimestamp(CMSDecoder, Int, UnsafeMutablePointer&lt;CFAbsoluteTime>) -> OSStatus

Returns the timestamp of a signer of a CMS message, if present.

func CMSDecoderCopySignerTimestampCertificates(CMSDecoder, Int, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Returns an array containing the certificates from a timestamp response.

func CMSDecoderCopySignerTimestampWithPolicy(CMSDecoder, CFTypeRef?, Int, UnsafeMutablePointer&lt;CFAbsoluteTime>) -> OSStatus

Returns the timestamp of a signer of a CMS message using a given policy, if present.

func CMSEncoderCopySignerTimestamp(CMSEncoder, Int, UnsafeMutablePointer&lt;CFAbsoluteTime>) -> OSStatus

Returns the timestamp of a signer of a CMS message, if present.

func CMSEncoderCopySignerTimestampWithPolicy(CMSEncoder, CFTypeRef?, Int, UnsafeMutablePointer&lt;CFAbsoluteTime>) -> OSStatus

Returns the timestamp of a signer of a CMS message using a particular policy, if present.

