

- Synchronization
-  Atomic 

Structure

# Atomic

An atomic value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct Atomic where Value : AtomicRepresentable
```

## Topics

### Initializers

init(consuming Value)

Initializes a value of this atomic with the given initial value.

### Instance Methods

func add(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func add(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic add operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseAnd(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic bitwise AND operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseOr(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic bitwise OR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func bitwiseXor(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic bitwise XOR operation and return the old and new value, applying the specified memory ordering.

func compareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified memory ordering.

func compareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified memory ordering.

func compareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified memory ordering.

func compareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified memory ordering.

func compareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified memory ordering.

func compareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified success/failure memory orderings.

func compareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified success/failure memory orderings.

func compareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified success/failure memory orderings.

func compareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified success/failure memory orderings.

func compareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic compare and exchange operation on the current value, applying the specified success/failure memory orderings.

func exchange(consuming Value, ordering: AtomicUpdateOrdering) -> Value

Atomically sets the current value to `desired` and returns the original value, applying the specified memory ordering.

func exchange(consuming Value, ordering: AtomicUpdateOrdering) -> Value

Atomically sets the current value to `desired` and returns the original value, applying the specified memory ordering.

func exchange(consuming Value, ordering: AtomicUpdateOrdering) -> Value

Atomically sets the current value to `desired` and returns the original value, applying the specified memory ordering.

func exchange(consuming Value, ordering: AtomicUpdateOrdering) -> Value

Atomically sets the current value to `desired` and returns the original value, applying the specified memory ordering.

func exchange(consuming Value, ordering: AtomicUpdateOrdering) -> Value

Atomically sets the current value to `desired` and returns the original value, applying the specified memory ordering.

func load(ordering: AtomicLoadOrdering) -> Value

Atomically loads and returns the current value, applying the specified memory ordering.

func load(ordering: AtomicLoadOrdering) -> Value

Atomically loads and returns the current value, applying the specified memory ordering.

func load(ordering: AtomicLoadOrdering) -> Value

Atomically loads and returns the current value, applying the specified memory ordering.

func load(ordering: AtomicLoadOrdering) -> Value

Atomically loads and returns the current value, applying the specified memory ordering.

func load(ordering: AtomicLoadOrdering) -> Value

Atomically loads and returns the current value, applying the specified memory ordering.

func logicalAnd(Bool, ordering: AtomicUpdateOrdering) -> (oldValue: Bool, newValue: Bool)

Perform an atomic logical AND operation and return the old and new value, applying the specified memory ordering.

func logicalOr(Bool, ordering: AtomicUpdateOrdering) -> (oldValue: Bool, newValue: Bool)

Perform an atomic logical OR operation and return the old and new value, applying the specified memory ordering.

func logicalXor(Bool, ordering: AtomicUpdateOrdering) -> (oldValue: Bool, newValue: Bool)

Perform an atomic logical XOR operation and return the old and new value, applying the specified memory ordering.

func max(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func max(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic maximum operation and return the old and new value, applying the specified memory ordering.

func min(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func min(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic minimum operation and return the old and new value, applying the specified memory ordering.

func store(consuming Value, ordering: AtomicStoreOrdering)

Atomically sets the current value to `desired`, applying the specified memory ordering.

func store(consuming Value, ordering: AtomicStoreOrdering)

Atomically sets the current value to `desired`, applying the specified memory ordering.

func store(consuming Value, ordering: AtomicStoreOrdering)

Atomically sets the current value to `desired`, applying the specified memory ordering.

func store(consuming Value, ordering: AtomicStoreOrdering)

Atomically sets the current value to `desired`, applying the specified memory ordering.

func store(consuming Value, ordering: AtomicStoreOrdering)

Atomically sets the current value to `desired`, applying the specified memory ordering.

func subtract(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func subtract(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic subtract operation and return the old and new value, applying the specified memory ordering.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the memory ordering. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the memory ordering. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the memory ordering. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the memory ordering. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, ordering: AtomicUpdateOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the memory ordering. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the specified success/failure memory orderings. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the specified success/failure memory orderings. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the specified success/failure memory orderings. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the specified success/failure memory orderings. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func weakCompareExchange(expected: consuming Value, desired: consuming Value, successOrdering: AtomicUpdateOrdering, failureOrdering: AtomicLoadOrdering) -> (exchanged: Bool, original: Value)

Perform an atomic weak compare and exchange operation on the current value, applying the specified success/failure memory orderings. This compare-exchange variant is allowed to spuriously fail; it is designed to be called in a loop until it indicates a successful exchange has happened.

func wrappingAdd(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingAdd(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic wrapping add operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(Int16, ordering: AtomicUpdateOrdering) -> (oldValue: Int16, newValue: Int16)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(Int64, ordering: AtomicUpdateOrdering) -> (oldValue: Int64, newValue: Int64)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(UInt128, ordering: AtomicUpdateOrdering) -> (oldValue: UInt128, newValue: UInt128)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(Int, ordering: AtomicUpdateOrdering) -> (oldValue: Int, newValue: Int)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(Int8, ordering: AtomicUpdateOrdering) -> (oldValue: Int8, newValue: Int8)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(UInt32, ordering: AtomicUpdateOrdering) -> (oldValue: UInt32, newValue: UInt32)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(UInt, ordering: AtomicUpdateOrdering) -> (oldValue: UInt, newValue: UInt)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(UInt64, ordering: AtomicUpdateOrdering) -> (oldValue: UInt64, newValue: UInt64)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(Int128, ordering: AtomicUpdateOrdering) -> (oldValue: Int128, newValue: Int128)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(UInt8, ordering: AtomicUpdateOrdering) -> (oldValue: UInt8, newValue: UInt8)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(UInt16, ordering: AtomicUpdateOrdering) -> (oldValue: UInt16, newValue: UInt16)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

func wrappingSubtract(Int32, ordering: AtomicUpdateOrdering) -> (oldValue: Int32, newValue: Int32)

Perform an atomic wrapping subtract operation and return the old and new value, applying the specified memory ordering.

## Relationships

### Conforms To

- Sendable

  Conforms when `Value` conforms to `Sendable` and `AtomicRepresentable`.

## See Also

### Atomic Values

struct AtomicLazyReference

A lazily initializable atomic strong reference.

struct WordPair

A pair of two word sized `UInt`s.

protocol AtomicRepresentable

A type that supports atomic operations through a separate atomic storage representation.

protocol AtomicOptionalRepresentable

An atomic value that also supports atomic operations when wrapped in an `Optional`. Atomic optional representable types come with a standalone atomic representation for their optional-wrapped variants.

