

- Core Services
- Apple Events
-  Constants for Object Specifiers, Positions, and Logical and Comparison Operations 

# Constants for Object Specifiers, Positions, and Logical and Comparison Operations

Specify the types of the four keyword-specified descriptors that make up the data in an object specifier, as well as constants for position, logical operations, and comparison operations.

## Overview

When you call the CreateLogicalDescriptor(_:_:_:_:) function to create a logical descriptor, you pass one of the logical operators `kAEAND`, `kAEOR`, or `kAENOT` in the `theLogicOperator` parameter. The `CreateLogicalDescriptor` function creates a logical descriptor that specifies a logical operation to perform on one or more operands.

The constants `kAEFirst`, `kAELast`, `kAEMiddle`, `kAEAny`, and `kAEAll` provide the key data for a keyword-specified descriptor of key form `formAbsolutePosition` and descriptor type `typeAbsoluteOrdinal`.

The constants `kAENext`, and `kAEPrevious` provide the key data for a keyword-specified descriptor of key form `formRelativePosition`.

Key form constants and descriptor type constants for object specifiers are defined in Key Form and Descriptor Type Object Specifier Constants.

The constants `keyAELogicalTerms` and `keyAELogicalOperator` define the keyword descriptors for a logical descriptor. A logical descriptor is a coerced Apple event record of type `typeLogicalDescriptor `that specifies a logical expression—that is, an expression that the Apple Event Manager evaluates to either `TRUE` or `FALSE`. You can create a logical descriptor with the CreateLogicalDescriptor(_:_:_:_:) function.

The data for a logical descriptor consists of two keyword-specified descriptors: the first with descriptor type `keyAELogicalOperator`, descriptor type `typeEnumerated`, and one of the logical operators defined in Constants for Object Specifiers, Positions, and Logical and Comparison Operations for its data; and the second with descriptor type `keyAELogicalTerms`, descriptor type `typeEnumerated`, and one or more comparison or logical descriptors for its data. Comparison constants are described in Comparison Operator Constants.

The logical expression is constructed from a logical operator (one of the Boolean operators `AND`, `OR`, or `NOT`) and a list of logical terms to which the operator is applied (where `NOT` can only be used where the list of terms is a single-item list). Each logical term in the list can be either another logical descriptor or a comparison descriptor (described in Constants for Object Specifiers, Positions, and Logical and Comparison Operations).

The Apple Event Manager short-circuits its evaluation of a logical expression as soon as one part of the expression fails a test. For example, if while testing a logical expression such as A `AND` B `AND` C the Apple Event Manager discovers that A `AND` B is not true, it will evaluate the expression to `FALSE` without testing C.

The constants `keyAECompOperator`, `keyAEObject1`, and `keyAEObject2` define the keyword descriptors for a comparison descriptor. A comparison descriptor is a coerced Apple event record of type `typeCompDescriptor` that specifies an Apple event object and either another Apple event object or data for the Apple Event Manager to compare to the first object. You can create a logical descriptor with the CreateCompDescriptor(_:_:_:_:_:) function.

The Apple Event Manager can also use the information in a comparison descriptor to compare elements in a container, one at a time, either to an Apple event object or to data. The data for a comparison descriptor consists of three keyword-specified descriptors:

- A descriptor with keyword `keyAECompOperator`, descriptor type `typeType`, and one of the logical operators defined in Comparison Operator Constants for its data.

- A descriptor with keyword `keyAEObject1` and either

- descriptor type `typeObjectSpecifier` and object specifier data to compare, or

- descriptor type `typeObjectBeingExamined` and a data storage pointer of `NULL`.

- A descriptor with keyword `keyAEObject2 `and either

- descriptor type `typeObjectSpecifier` and object specifier data to compare, or

- descriptor type `typeObjectBeingExamined` and a data storage pointer of `NULL`, or

- any other descriptor type and the data to be compared for that descriptor type.

You don’t have to support all the available comparison operators for all Apple event objects for example, the `beginswith` operator probably doesn’t make sense for objects of type `cRectangle`. It is up to you to decide which comparison operators are appropriate for your application to support, and how to interpret them. If necessary, you can define your own custom comparison operators. If you think you need to do this, check the Apple Events and Scripting header files to see if existing definitions of comparison operators can be adapted to the needs of your application.

An object specifier is a coerced Apple event record of descriptor type `typeObjectSpecifier` whose data contains consists of four keyword-specified descriptors. The constants `keyAEDesiredClass`, `keyAEContainer`, `keyAEKeyForm`, and `keyAEKeyData` specify the keywords for the four descriptor types that together identify the specified object or objects.

## Topics

### Constants

var kAEAND: Int

Specifies a logical `AND` operation.

var kAEOR: Int

Specifies a logical `OR` operation.

var kAENOT: Int

Specifies a logical `NOT` operation.

var kAEFirst: Int

The first element in the specified container.

var kAELast: Int

Specifies the last element in the container.

var kAEMiddle: Int

var kAEAny: Int

Specifies a single element chosen at random from the container.

var kAEAll: Int

Specifies all the elements in the container.

var kAENext: Int

Specifies the Apple event object after the container.

var kAEPrevious: Int

Specifies the Apple event object before the container.

var keyAECompOperator: Int

Specifies a descriptor of `typeType`, whose data consists of one of the constant values described in Key Form and Descriptor Type Object Specifier Constants.

var keyAELogicalTerms: Int

Specifies a descriptor of type `typeAEList` containing one or more comparison or logical descriptors.

var keyAELogicalOperator: Int

Specifies a descriptor of type `typeEnumerated` whose data is one of the logical operators (such as `kAEAND`) defined in Key Form and Descriptor Type Object Specifier Constants.

var keyAEObject1: Int

var keyAEObject2: Int

var keyAEDesiredClass: Int

var keyAEContainer: Int

Specifies the container for the requested object or objects. The data is an object specifier (or in some cases a null descriptor).

var keyAEKeyForm: Int

var keyAEKeyData: Int

