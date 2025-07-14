

- Swift Testing
- CustomTestArgumentEncodable
-  encodeTestArgument(to:) 

Instance Method

# encodeTestArgument(to:)

Encode this test argument.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
func encodeTestArgument(to encoder: some Encoder) throws
```

**Required**

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

Throws

Any error encountered during encoding.

The encoded form of a test argument should be stable and unique to allow re-running specific test cases of a parameterized test function. For optimal performance, large values which are not necessary to uniquely identify the test argument later should be omitted. Encoded values do not need to be human-readable.

For more information on how to implement this function, see the documentation for Encodable.

