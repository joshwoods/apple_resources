

- Foundation
- Numbers, Data, and Basic Values
- Data
-  DataProtocol Implementations 

API Collection

# DataProtocol Implementations

## Topics

### Instance Methods

func copyBytes(to: UnsafeMutableRawBufferPointer) -> Int

func copyBytes&lt;DestinationType>(to: UnsafeMutableBufferPointer&lt;DestinationType>) -> Int

func firstRange&lt;D>(of: D) -> Range&lt;Self.Index>?

func firstRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the first found range of the given data buffer.

func lastRange&lt;D>(of: D) -> Range&lt;Self.Index>?

func lastRange&lt;D, R>(of: D, in: R) -> Range&lt;Self.Index>?

Returns the last found range of the given data buffer.

