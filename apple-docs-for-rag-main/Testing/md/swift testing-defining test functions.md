

- Swift Testing
-  Defining test functions 

Article

# Defining test functions

Define a test function to validate that code is working correctly.

## Overview

Defining a test function for a Swift package or project is straightforward.

### Import the testing library

To import the testing library, add the following to the Swift source file that contains the test:

```
```

Note

Only import the testing library into a test target. Importing the testing library into an application, library, or binary target isn’t supported or recommended. Test functions aren’t stripped from binaries when building for release, so logic and fixtures of a test may be visible to anyone who inspects a build product that contains a test function.

### Declare a test function

To declare a test function, write a Swift function declaration that doesn’t take any arguments, then prefix its name with the `@Test` attribute:

```
```

This test function can be present at file scope or within a type. A type containing test functions is automatically a *test suite* and can be optionally annotated with the `@Suite` attribute. For more information about suites, see Organizing test functions with suite types.

Note that, while this function is a valid test function, it doesn’t actually perform any action or test any code. To check for expected values and outcomes in test functions, add expectations to the test function.

### Customize a test’s name

To customize a test function’s name as presented in an IDE or at the command line, supply a string literal as an argument to the `@Test` attribute:

```
```

To further customize the appearance and behavior of a test function, use traits such as tags(_:).

### Write concurrent or throwing tests

As with other Swift functions, test functions can be marked `async` and `throws` to annotate them as concurrent or throwing, respectively. If a test is only safe to run in the main actor’s execution context (that is, from the main thread of the process), it can be annotated `@MainActor`:

```
```

### Limit the availability of a test

If a test function can only run on newer versions of an operating system or of the Swift language, use the `@available` attribute when declaring it. Use the `message` argument of the `@available` attribute to specify a message to log if a test is unable to run due to limited availability:

```
```

## See Also

### Essentials

Organizing test functions with suite types

Organize tests into test suites.

Migrating a test from XCTest

Migrate an existing test method or test class written using XCTest.

macro Test(String?, any TestTrait...)

Declare a test.

struct Test

A type representing a test or suite.

macro Suite(String?, any SuiteTrait...)

Declare a test suite.

