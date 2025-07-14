

- Security
-  ASN.1 

API Collection

# ASN.1

Encode and decode Distinguished Encoding Rules (DER) and Basic Encoding Rules (BER) data streams.

## Overview

You use an ASN.1 coder to encode and decode both DER and BER data streams based on templates that you supply, which in turn are based upon ASN.1 specifications. You must import this API explicitly:

- Swift
- Objective-C

```
import Security.SecAsn1Coder
import Security.SecAsn1Templates
```

```
#import 
#import 
```

## Topics

### Encoding

typealias SecAsn1Item

A structure holding DER encoded data.

Deprecated

struct SecAsn1Template_struct

A structure that defines one element of a BER or DER encoding.

Deprecated

struct SecAsn1Template_struct

A structure that defines one element of a BER or DER encoding.

Deprecated

typealias SecAsn1TemplateChooser

Dynamically provides the sub-template to use during encode or decode.

Deprecated

typealias SecAsn1TemplateChooserPtr

A pointer to the template chooser function.

Deprecated

Type Tags

Recognize BER and DER values for ASN.1 identifier octets.

### OID Comparison

typealias SecAsn1Oid

An object identifier.

Deprecated

### Public Key Info

struct SecAsn1AlgId

A structure identifying an ASN.1 algorithm by its OID, and its corresponding parameters.

Deprecated

struct SecAsn1PubKeyInfo

A structure containing a public key and its associated algorithm.

Deprecated

