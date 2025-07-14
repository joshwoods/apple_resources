

- Foundation
- NSArchiver
-  classNameEncoded(forTrueClassName:) Deprecated

Instance Method

# classNameEncoded(forTrueClassName:)

Returns the name of the class used to archive instances of the class with a given true name.

iOS 2.0–11.0DeprecatediPadOS 2.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.13Deprecated

``` source
func classNameEncoded(forTrueClassName trueName: String) -> String?
```

Deprecated

Use NSKeyedArchiver instead

## Parameters 

`trueName`  

The real name of an encoded class.

## Return Value

The name of the class used to archive instances of the class `trueName`.

## See Also

### Substituting classes or objects

func encodeClassName(String, intoClassName: String)

Encodes a substitute name for the class with a given true name.

Deprecated

func replace(Any, with: Any)

Causes the receiver to treat subsequent requests to encode a given object as though they were requests to encode another given object.

Deprecated

