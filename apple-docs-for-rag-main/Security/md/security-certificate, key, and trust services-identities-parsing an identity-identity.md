

- Security
- Certificate, Key, and Trust Services
- Identities
-  Parsing an Identity 

Article

# Parsing an Identity

Extract the private key and certificate from an identity.

## Overview

After you have an identity, you can extract the private key from it with a call to the SecIdentityCopyPrivateKey(_:_:) function:

- Swift
- Objective-C

```
var privateKey: SecKey?
let status = SecIdentityCopyPrivateKey(identity, &privateKey)
guard status == errSecSuccess else { throw  }
```

```
SecKeyRef privateKey = NULL;
OSStatus status = SecIdentityCopyPrivateKey(identity,
                                            &privateKey);
if (status != errSecSuccess) {  }
else                         {  }

if (privateKey)  { CFRelease(privateKey); } // After you are done with it
```

Similarly, you can extract the certificate with a call to the SecIdentityCopyCertificate(_:_:) function:

- Swift
- Objective-C

```
var certificate: SecCertificate?
let status = SecIdentityCopyCertificate(identity, &certificate)
guard status == errSecSuccess else { throw  }
```

```
SecCertificateRef certificate = NULL;
OSStatus status = SecIdentityCopyCertificate(identity,
                                             &certificate);
if (status != errSecSuccess) {  }
else                         {  }

if (certificate) { CFRelease(certificate); }  // After you are done with it
```

In both cases, you inspect the returned status value to determine whether an error occurred during the extraction. In Objective-C, you are responsible for freeing the associated memory with a call to CFRelease when you’re done with these objects. In Swift, the system manages the memory automatically, releasing it when the object goes out of scope.

