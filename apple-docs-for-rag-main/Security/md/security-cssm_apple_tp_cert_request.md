

- Security
-  CSSM_APPLE_TP_CERT_REQUEST 

Structure

# CSSM_APPLE_TP_CERT_REQUEST

macOS 10.0+

``` source
struct CSSM_APPLE_TP_CERT_REQUEST
```

## Topics

### Initializers

init()

init(cspHand: CSSM_CSP_HANDLE, clHand: CSSM_CL_HANDLE, serialNumber: uint32, numSubjectNames: uint32, subjectNames: UnsafeMutablePointer&lt;CSSM_APPLE_TP_NAME_OID>!, numIssuerNames: uint32, issuerNames: UnsafeMutablePointer&lt;CSSM_APPLE_TP_NAME_OID>!, issuerNameX509: UnsafeMutablePointer&lt;cssm_x509_name>!, certPublicKey: UnsafePointer&lt;cssm_key>!, issuerPrivateKey: UnsafePointer&lt;cssm_key>!, signatureAlg: CSSM_ALGORITHMS, signatureOid: SecAsn1Oid, notBefore: uint32, notAfter: uint32, numExtensions: uint32, extensions: UnsafeMutablePointer&lt;__CE_DataAndType>!, challengeString: UnsafePointer&lt;CChar>!)

### Instance Properties

var certPublicKey: UnsafePointer&lt;cssm_key>!

var challengeString: UnsafePointer&lt;CChar>!

var clHand: CSSM_CL_HANDLE

var cspHand: CSSM_CSP_HANDLE

var extensions: UnsafeMutablePointer&lt;__CE_DataAndType>!

var issuerNameX509: UnsafeMutablePointer&lt;cssm_x509_name>!

var issuerNames: UnsafeMutablePointer&lt;CSSM_APPLE_TP_NAME_OID>!

var issuerPrivateKey: UnsafePointer&lt;cssm_key>!

var notAfter: uint32

var notBefore: uint32

var numExtensions: uint32

var numIssuerNames: uint32

var numSubjectNames: uint32

var serialNumber: uint32

var signatureAlg: CSSM_ALGORITHMS

var signatureOid: SecAsn1Oid

var subjectNames: UnsafeMutablePointer&lt;CSSM_APPLE_TP_NAME_OID>!

## Relationships

### Conforms To

- BitwiseCopyable

