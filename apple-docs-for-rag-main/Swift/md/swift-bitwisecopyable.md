

- Swift
-  BitwiseCopyable 

Protocol

# BitwiseCopyable

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol BitwiseCopyable : ~Escapable
```

## Relationships

### Inherited By

- SIMDScalar

### Conforming Types

- AtomicLoadOrdering
- AtomicStoreOrdering
- AtomicUpdateOrdering
- AutoreleasingUnsafeMutablePointer
- Bool
- CVaListPointer
- CollectionDifference.Index

  Conforms when `ChangeElement` conforms to `Copyable` and `Escapable`.

- DiscardingTaskGroup
- Double
- Double.SIMD16Storage
- Double.SIMD2Storage
- Double.SIMD32Storage
- Double.SIMD4Storage
- Double.SIMD64Storage
- Double.SIMD8Storage
- Duration
- EmptyCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- EmptyCollection.Iterator

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Float
- Float.SIMD16Storage
- Float.SIMD2Storage
- Float.SIMD32Storage
- Float.SIMD4Storage
- Float.SIMD64Storage
- Float.SIMD8Storage
- Float16
- Float16.SIMD16Storage
- Float16.SIMD2Storage
- Float16.SIMD32Storage
- Float16.SIMD4Storage
- Float16.SIMD64Storage
- Float16.SIMD8Storage
- Float80
- FloatingPointClassification
- FloatingPointSign
- Hasher
- Int
- Int.SIMD16Storage
- Int.SIMD2Storage
- Int.SIMD32Storage
- Int.SIMD4Storage
- Int.SIMD64Storage
- Int.SIMD8Storage
- Int.Words
- Int128
- Int16
- Int16.SIMD16Storage
- Int16.SIMD2Storage
- Int16.SIMD32Storage
- Int16.SIMD4Storage
- Int16.SIMD64Storage
- Int16.SIMD8Storage
- Int16.Words
- Int32
- Int32.SIMD16Storage
- Int32.SIMD2Storage
- Int32.SIMD32Storage
- Int32.SIMD4Storage
- Int32.SIMD64Storage
- Int32.SIMD8Storage
- Int32.Words
- Int64
- Int64.SIMD16Storage
- Int64.SIMD2Storage
- Int64.SIMD32Storage
- Int64.SIMD4Storage
- Int64.SIMD64Storage
- Int64.SIMD8Storage
- Int64.Words
- Int8
- Int8.SIMD16Storage
- Int8.SIMD2Storage
- Int8.SIMD32Storage
- Int8.SIMD4Storage
- Int8.SIMD64Storage
- Int8.SIMD8Storage
- Int8.Words
- JobPriority
- Never
- ObjectIdentifier
- OpaquePointer
- Optional

  Conforms when `Wrapped` conforms to `BitwiseCopyable` and `Escapable`.

- SIMD16

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD16Storage` conforms to `BitwiseCopyable`.

- SIMD2

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD2Storage` conforms to `BitwiseCopyable`.

- SIMD3

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD4Storage` conforms to `BitwiseCopyable`.

- SIMD32

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD32Storage` conforms to `BitwiseCopyable`.

- SIMD4

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD4Storage` conforms to `BitwiseCopyable`.

- SIMD64

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD64Storage` conforms to `BitwiseCopyable`.

- SIMD8

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD8Storage` conforms to `BitwiseCopyable`.

- StaticBigInt
- StaticString
- String.Index
- SystemRandomNumberGenerator
- TaskGroup

  Conforms when `ChildTaskResult` conforms to `Copyable`, `Escapable`, and `Sendable`.

- ThrowingDiscardingTaskGroup

  Conforms when `Failure` conforms to `Error`.

- ThrowingTaskGroup

  Conforms when `ChildTaskResult` conforms to `Copyable`, `ChildTaskResult` conforms to `Escapable`, `ChildTaskResult` conforms to `Sendable`, and `Failure` conforms to `Error`.

- UInt
- UInt.SIMD16Storage
- UInt.SIMD2Storage
- UInt.SIMD32Storage
- UInt.SIMD4Storage
- UInt.SIMD64Storage
- UInt.SIMD8Storage
- UInt.Words
- UInt128
- UInt128.Words
- UInt16
- UInt16.SIMD16Storage
- UInt16.SIMD2Storage
- UInt16.SIMD32Storage
- UInt16.SIMD4Storage
- UInt16.SIMD64Storage
- UInt16.SIMD8Storage
- UInt16.Words
- UInt32
- UInt32.SIMD16Storage
- UInt32.SIMD2Storage
- UInt32.SIMD32Storage
- UInt32.SIMD4Storage
- UInt32.SIMD64Storage
- UInt32.SIMD8Storage
- UInt32.Words
- UInt64
- UInt64.SIMD16Storage
- UInt64.SIMD2Storage
- UInt64.SIMD32Storage
- UInt64.SIMD4Storage
- UInt64.SIMD64Storage
- UInt64.SIMD8Storage
- UInt64.Words
- UInt8
- UInt8.SIMD16Storage
- UInt8.SIMD2Storage
- UInt8.SIMD32Storage
- UInt8.SIMD4Storage
- UInt8.SIMD64Storage
- UInt8.SIMD8Storage
- UInt8.Words
- UnboundedRange_
- Unicode.ASCII
- Unicode.ASCII.Parser
- Unicode.Scalar
- Unicode.Scalar.UTF16View
- Unicode.Scalar.UTF8View
- Unicode.UTF16
- Unicode.UTF16.ForwardParser
- Unicode.UTF16.ReverseParser
- Unicode.UTF32
- Unicode.UTF32.Parser
- Unicode.UTF8
- Unicode.UTF8.ForwardParser
- Unicode.UTF8.ReverseParser
- UnicodeDecodingResult
- Unmanaged

  Conforms when `Instance` conforms to `Copyable` and `Escapable`.

- UnownedJob
- UnownedSerialExecutor
- UnownedTaskExecutor
- UnsafeBufferPointer

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- UnsafeContinuation

  Conforms when `T` conforms to `Copyable`, `T` conforms to `Escapable`, and `E` conforms to `Error`.

- UnsafeMutableBufferPointer

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- UnsafeMutablePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeMutableRawBufferPointer
- UnsafeMutableRawPointer
- UnsafePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeRawBufferPointer
- UnsafeRawBufferPointer.Iterator
- UnsafeRawPointer
- WordPair

## See Also

### Copying

protocol Copyable

A type whose values can be implicitly or explicitly copied.

