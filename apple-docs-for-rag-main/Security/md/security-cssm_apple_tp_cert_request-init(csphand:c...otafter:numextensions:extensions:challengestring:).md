

- Security
- CSSM_APPLE_TP_CERT_REQUEST
-  init(cspHand:clHand:serialNumber:numSubjectNames:subjectNames:numIssuerNames:issuerNames:issuerNameX509:certPublicKey:issuerPrivateKey:signatureAlg:signatureOid:notBefore:notAfter:numExtensions:extensions:challengeString:) 

Initializer

# init(cspHand:clHand:serialNumber:numSubjectNames:subjectNames:numIssuerNames:issuerNames:issuerNameX509:certPublicKey:issuerPrivateKey:signatureAlg:signatureOid:notBefore:notAfter:numExtensions:extensions:challengeString:)

macOS 10.0+

``` source
init(
    cspHand: CSSM_CSP_HANDLE,
    clHand: CSSM_CL_HANDLE,
    serialNumber: uint32,
    numSubjectNames: uint32,
    subjectNames: UnsafeMutablePointer!,
    numIssuerNames: uint32,
    issuerNames: UnsafeMutablePointer!,
    issuerNameX509: UnsafeMutablePointer!,
    certPublicKey: UnsafePointer!,
    issuerPrivateKey: UnsafePointer!,
    signatureAlg: CSSM_ALGORITHMS,
    signatureOid: SecAsn1Oid,
    notBefore: uint32,
    notAfter: uint32,
    numExtensions: uint32,
    extensions: UnsafeMutablePointer!,
    challengeString: UnsafePointer!
)
```

