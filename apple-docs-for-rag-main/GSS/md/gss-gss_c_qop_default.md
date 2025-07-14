

- GSS
-  GSS_C_QOP_DEFAULT 

Global Variable

# GSS_C_QOP_DEFAULT

The default Quality of Protection for per-message services.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var GSS_C_QOP_DEFAULT: Int32 { get }
```

## Discussion

An implementation that offers multiple levels of QOP may define this value to be either zero (as done here) to mean “default protection,” or to a specific explicit QOP value. However, a value of 0 is always interpreted by a GSS-API implementation as a request for the default protection level.

## See Also

### Quality of Protection Constants

var GSS_KRB5_CONF_C_QOP_DES: Int32

The Kerberos 5 Qualty of Service 56-bit DES encryption.

var GSS_KRB5_CONF_C_QOP_DES3_KD: Int32

The Kerberos 5 Qualty of Service 168-bit DES3 encryption with key derivation.

