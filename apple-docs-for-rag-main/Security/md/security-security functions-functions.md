

- Security
-  Security Functions 

API Collection

# Security Functions

## Topics

### Functions

func SecCertificateCopyNotValidAfterDate(SecCertificate) -> CFDate?

func SecCertificateCopyNotValidBeforeDate(SecCertificate) -> CFDate?

func SecCodeCreateWithXPCMessage(xpc_object_t, SecCSFlags, UnsafeMutablePointer&lt;SecCode?>) -> OSStatus

func SecCodeValidateFileResource(SecStaticCode, CFString, CFData, SecCSFlags) -> OSStatus

func SecTaskGetCodeSignStatus(SecTask) -> UInt32

func SecTrustCopyCertificateChain(SecTrust) -> CFArray?

func SecTrustCopyKey(SecTrust) -> SecKey?

