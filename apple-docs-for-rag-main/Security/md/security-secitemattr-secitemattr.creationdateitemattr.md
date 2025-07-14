

- Security
- SecItemAttr
-  SecItemAttr.creationDateItemAttr 

Case

# SecItemAttr.creationDateItemAttr

Identifies the creation date attribute.

Mac Catalyst 13.0+macOS 10.0+

``` source
case creationDateItemAttr
```

## Discussion

You use this tag to get a string value that represents the date the item was created, expressed in Zulu Time format (“YYYYMMDDhhmmssZ”). This is the native format for stored time values in the CDSA specification (defined as `CSSM_DB_ATTRIBUTE_FORMAT_TIME_DATE` in the `CSSM_DB_ATTRIBUTE_FORMAT` enumeration, Section 17.2.6.). When specifying the creation date as input to a function (for example, SecKeychainSearchCreateFromAttributes), you may alternatively provide a numeric value of type `UInt32` or `SInt64`, expressed as seconds since 01 January 1904.

