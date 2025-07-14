

- Security
-  kSecCodeInfoTimestamp 

Global Variable

# kSecCodeInfoTimestamp

A key whose value indicates the actual signing date.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoTimestamp: CFString
```

## Discussion

The value is a CFDate object describing the signing date as (securely) certified by a timestamp authority service. This timestamp cannot be falsified by the signer, and is trusted to the same degree as the timestamp service that created the timestamp.

