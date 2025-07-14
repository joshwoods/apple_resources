

- XCTest
-  XCTActivity 

Protocol

# XCTActivity

A named substep of a test method.

``` source
protocol XCTActivity : NSObjectProtocol
```

## Mentioned in 

Adding Attachments to Tests, Activities, and Issues

## Topics

### Adding Attachments

func add(XCTAttachment)

Associates a file, image, or other attachment with the activity.

**Required**

### Activity Properties

var name: String

A human-readable name for the activity.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- XCTestCase

## See Also

### Activities

Grouping Tests into Substeps with Activities

Simplify test reports by creating activities that organize substeps within complex test methods.

class XCTContext

A proxy for the current testing context.

