

- XCTest
- XCTActivity
-  name 

Instance Property

# name

A human-readable name for the activity.

``` source
var name: String { get }
```

**Required**

## Discussion

The activity’s name is used to group the activity within test output in Xcode test reports.

For activities created with the XCTContext runActivityNamed:block: class method, the name property will match the `name` parameter passed to the class method.

