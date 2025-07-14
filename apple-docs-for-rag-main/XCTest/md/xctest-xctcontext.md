

- XCTest
-  XCTContext 

Class

# XCTContext

A proxy for the current testing context.

``` source
class XCTContext
```

## Mentioned in 

Grouping Tests into Substeps with Activities

Adding Attachments to Tests, Activities, and Issues

## Overview

`XCTContext` provides a way for activities (XCTActivity) to run against the current testing context, either directly in a test case or in custom testing utilities. You can break up long test methods in UI tests or integration tests into activities to reuse, and to simplify results in the Xcode test reports. Use runActivity(named:block:) to run a block of code as a named substep in a test. For more information, see Grouping Tests into Substeps with Activities.

## Topics

### Running Activities

class func runActivity&lt;Result>(named: String, block: (any XCTActivity) throws -> Result) rethrows -> Result

Creates and runs an activity with the provided block of code.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Activities

Grouping Tests into Substeps with Activities

Simplify test reports by creating activities that organize substeps within complex test methods.

protocol XCTActivity

A named substep of a test method.

