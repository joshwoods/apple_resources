

- Security
- CMSSignedAttributes
-  attrSmimeCapabilities 

Type Property

# attrSmimeCapabilities

Identify signature, encryption, and digest algorithms supported by the encoder.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var attrSmimeCapabilities: CMSSignedAttributes { get }
```

## Discussion

Using this attribute doesn’t change the encoding. See RFC 2311: S/MIME Version 2 Message Specification section 2.5.2 for more information about the capabilities attribute.

