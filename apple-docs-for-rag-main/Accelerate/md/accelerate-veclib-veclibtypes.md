

- Accelerate
- vecLib
-  vecLibTypes 

API Collection

# vecLibTypes

Create and work with 128-bit vector data types.

## Overview

The vecLibTypes.h header file defines a set of vector data types (`vFloat`, `vUInt32`, etc.), which represent 128-bit vectors containing values of type `float`, `UInt32`, etc. The vBasicOps.h and vfp.h headers make use of these types.

The type names all begin with the letter “v,” followed by a mnemonic for the scalar data type used for elements of the vector. For example, `vUInt32`, `vSInt16`, `vFloat`, etc.

## Topics

### Type Aliases

typealias la_attribute_t

typealias la_count_t

typealias la_deallocator_t

typealias la_hint_t

typealias la_index_t

typealias la_norm_t

typealias la_object_t

typealias la_scalar_type_t

typealias la_status_t

protocol OS_la_object

### vecLibTypes

typealias vUInt8

A 128-bit vector packed with `unsigned char` values.

typealias vSInt8

A 128-bit vector packed with `signed char` values.

typealias vUInt16

A 128-bit vector packed with `unsigned short` values.

typealias vSInt16

A 128-bit vector packed with `signed short` values.

typealias vUInt32

A 128-bit vector packed with `unsigned int` values.

typealias vSInt32

A 128-bit vector packed with `signed int` values.

typealias vUInt64

A 128-bit vector packed with `uint64_t` values.

typealias vSInt64

A 128-bit vector packed with `int64_t` values.

typealias vFloat

A 128-bit vector packed with `float` values.

typealias vDouble

A 128-bit vector packed with `double` values.

typealias vBool32

A 128-bit vector packed with `bool int` values.

