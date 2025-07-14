

- Security
- CSSM_APPLE_CL_CSR_REQUEST
-  init(subjectNameX509:signatureAlg:signatureOid:cspHand:subjectPublicKey:subjectPrivateKey:challengeString:) 

Initializer

# init(subjectNameX509:signatureAlg:signatureOid:cspHand:subjectPublicKey:subjectPrivateKey:challengeString:)

macOS 10.0+

``` source
init(
    subjectNameX509: UnsafeMutablePointer!,
    signatureAlg: CSSM_ALGORITHMS,
    signatureOid: SecAsn1Oid,
    cspHand: CSSM_CSP_HANDLE,
    subjectPublicKey: UnsafePointer!,
    subjectPrivateKey: UnsafePointer!,
    challengeString: UnsafePointer!
)
```

