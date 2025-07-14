

- Security
-  CSSM_APPLE_CL_CSR_REQUEST 

Structure

# CSSM_APPLE_CL_CSR_REQUEST

macOS 10.0+

``` source
struct CSSM_APPLE_CL_CSR_REQUEST
```

## Topics

### Initializers

init()

init(subjectNameX509: UnsafeMutablePointer&lt;cssm_x509_name>!, signatureAlg: CSSM_ALGORITHMS, signatureOid: SecAsn1Oid, cspHand: CSSM_CSP_HANDLE, subjectPublicKey: UnsafePointer&lt;cssm_key>!, subjectPrivateKey: UnsafePointer&lt;cssm_key>!, challengeString: UnsafePointer&lt;CChar>!)

### Instance Properties

var challengeString: UnsafePointer&lt;CChar>!

var cspHand: CSSM_CSP_HANDLE

var signatureAlg: CSSM_ALGORITHMS

var signatureOid: SecAsn1Oid

var subjectNameX509: UnsafeMutablePointer&lt;cssm_x509_name>!

var subjectPrivateKey: UnsafePointer&lt;cssm_key>!

var subjectPublicKey: UnsafePointer&lt;cssm_key>!

## Relationships

### Conforms To

- BitwiseCopyable

