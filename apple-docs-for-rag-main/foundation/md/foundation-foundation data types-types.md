

- Foundation
-  Foundation Data Types 

API Collection

# Foundation Data Types

This document describes the data types and constants found in the Foundation framework.

## Topics

### Classes

class NSKeyValueObservation

class NSKeyValueSharedObservers

class NSKeyValueSharedObserversSnapshot

### Protocols

protocol DiscreteFormatStyle

protocol NSKeyValueObservingCustomization

Conforming to NSKeyValueObservingCustomization is not required to use Key-Value Observing. Provide an implementation of these functions if you need to disable auto-notifying for a key, or add dependent keys

### Structures

struct AsyncCharacterSequence

An asynchronous sequence of characters.

struct AsyncLineSequence

An asynchronous sequence of lines of text.

struct AsyncUnicodeScalarSequence

An asychronous sequence of Unicode scalar values.

struct Expression

struct NSAttributedStringFormattingContextKey

struct NSKeyValueChangeKey

The keys that can appear in the change dictionary.

struct NSKeyValueObservedChange

struct NSKeyValueOperator

These constants define the available array operators. See Using Collection Operators for more information.

struct PresentationIntent

A type that defines presentation intent for blocks of characters like paragraphs, lists, block quotes, and tables.

### Variables

let NSOperationNotSupportedForKeyException: String

let NSURLSessionUploadTaskResumeData: String

var kCFStringEncodingASCII: CFStringEncoding

### Macros

macro Expression&lt;each Input, Output>((repeat each Input) -> Output) -> Expression&lt;repeat each Input, Output>

macro Predicate&lt;each Input>((repeat each Input) -> Bool) -> Predicate&lt;repeat each Input>

### Type Aliases

typealias uuid_string_t

typealias uuid_t

## See Also

### Reference

Foundation Enumerations

