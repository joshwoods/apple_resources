

- Security
- Certificate, Key, and Trust Services
- Certificates
-  Storing a DER-Encoded X.509 Certificate 

Article

# Storing a DER-Encoded X.509 Certificate

Import and export a certificate from a file.

## Overview

Certificates are not secret and you often want to share them to disseminate a public key, but SecCertificate is an opaque type that you can’t distribute directly. Instead, you create a Distinguished Encoding Rules (DER) encoded data representation of the certificate using the SecCertificateCopyData(_:) function:

- Swift
- Objective-C

```
let certificate = 
let certData = SecCertificateCopyData(certificate) as Data
```

```
SecCertificateRef certificate = ;
NSData* certData = (NSData*)CFBridgingRelease( // ARC takes ownership
                       SecCertificateCopyData(certificate)
                    );
```

You might send this data object over a network connection or store it in a `.cer` file:

- Swift
- Objective-C

```
certData.write(to: )
```

```
[certData writeToURL: atomically:YES];
```

When you receive such a data object, you use the SecCertificateCreateWithData(_:_:) function to reverse the process:

- Swift
- Objective-C

```
let certificate = SecCertificateCreateWithData(nil, certData as CFData)
```

```
SecCertificateRef certificate =
    SecCertificateCreateWithData(NULL, (__bridge CFDataRef)certData);

if (certificate)  { CFRelease(certificate); } // After you are done with it
```

By leaving the first argument empty, you rely on the default allocator to allocate memory for the certificate. Note that in Objective-C, you call CFRelease to free the certificate’s memory when you are done with it. In Swift, the system manages the object’s memory automatically.

