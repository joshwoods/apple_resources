

- Security
-  cssm_parsed_cert 

Structure

# cssm_parsed_cert

Mac Catalyst 13.0+macOS 10.0+

``` source
struct cssm_parsed_cert
```

## Topics

### Initializers

init()

init(CertType: CSSM_CERT_TYPE, ParsedCertFormat: CSSM_CERT_PARSE_FORMAT, ParsedCert: UnsafeMutableRawPointer!)

### Instance Properties

var CertType: CSSM_CERT_TYPE

var ParsedCert: UnsafeMutableRawPointer!

var ParsedCertFormat: CSSM_CERT_PARSE_FORMAT

## Relationships

### Conforms To

- BitwiseCopyable

