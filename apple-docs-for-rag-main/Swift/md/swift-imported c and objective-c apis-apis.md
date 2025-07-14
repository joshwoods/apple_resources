

- Swift
-  Imported C and Objective-C APIs 

# Imported C and Objective-C APIs

Use native Swift syntax to interoperate with types and functions in C and Objective-C.

## Overview

You can access and use pieces of code written in C and Objective-C from within your Swift code. After you import an Objective-C framework, a C library, or a header file, you can work with Objective-C classes and protocols, as well as common C constructs, functions, and patterns.

## Topics

### Swift and Objective-C in the Same Project

Access your Swift code from within your Objective-C codebase, and your Objective-C code from Swift.

Importing Objective-C into Swift

Access classes and other declarations from your Objective-C code in Swift.

Importing Swift into Objective-C

Access Swift types and declarations from within your Objective-C codebase.

### Cocoa Frameworks

Working with Foundation Types

Use bridged Foundation types in your Swift codebase to work with dates, times, and other values.

Working with Core Foundation Types

Work directly with memory-managed Core Foundation types in your Swift code, and manually handle retains as needed.

### Objective-C APIs

Using Imported Lightweight Generics in Swift

Understand the constraints of imported Obj-C lightweight generic type declarations.

Using Imported Protocol-Qualified Classes in Swift

Learn how imported Objective-C protocol-qualified classes and metaclasses are represented.

### C APIs

Using Imported C Structs and Unions in Swift

Learn how Swift represents imported C structures and unions, including types with bitfields and unnamed fields.

Using Imported C Functions in Swift

Learn how to call imported functions that are declared in a C header.

Using Imported C Macros in Swift

Use imported C-defined macros as constants.

## See Also

### Language Interoperability with Objective-C and C

Objective-C and C Code Customization

Apply macros to your Objective-C APIs to customize how they’re imported into Swift.

Migrating Your Objective-C Code to Swift

Learn the recommended steps to migrate your code.

Cocoa Design Patterns

Adopt and interoperate with Cocoa design patterns in your Swift apps.

Handling Dynamically Typed Methods and Objects in Swift

Cast instances of the Objective-C `id` type to a specific Swift type.

Using Objective-C Runtime Features in Swift

Use selectors and key paths to interact with dynamic Objective-C APIs.

Calling Objective-C APIs Asynchronously

Learn how functions and methods that take a completion handler are converted to Swift asynchronous functions.

