

- Security
-  cssm_parsed_crl 

Structure

# cssm_parsed_crl

Mac Catalyst 13.0+macOS 10.0+

``` source
struct cssm_parsed_crl
```

## Topics

### Initializers

init()

init(CrlType: CSSM_CRL_TYPE, ParsedCrlFormat: CSSM_CRL_PARSE_FORMAT, ParsedCrl: UnsafeMutableRawPointer!)

### Instance Properties

var CrlType: CSSM_CRL_TYPE

var ParsedCrl: UnsafeMutableRawPointer!

var ParsedCrlFormat: CSSM_CRL_PARSE_FORMAT

## Relationships

### Conforms To

- BitwiseCopyable

