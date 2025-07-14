

- Swift
- Swift Standard Library
- Encoding, Decoding, and Serialization
- KeyedEncodingContainer
-  KeyedEncodingContainerProtocol Implementations 

API Collection

# KeyedEncodingContainerProtocol Implementations

## Topics

### Instance Methods

func encode(Int128, forKey: Self.Key) throws

Encodes the given value for the given key.

func encode(UInt128, forKey: Self.Key) throws

Encodes the given value for the given key.

func encodeConditional&lt;T>(T, forKey: Self.Key) throws

Encodes a reference to the given object only if it is encoded unconditionally elsewhere in the payload (previously, or in the future).

func encodeIfPresent(UInt16?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Double?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt128?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int32?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent&lt;T>(T?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int16?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Bool?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int8?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt64?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(String?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt32?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int128?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Float?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt8?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int64?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

