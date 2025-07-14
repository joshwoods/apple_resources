

- XCTest
- XCTestLog
-  testLog(withFormat:arguments:) 

Instance Method

# testLog(withFormat:arguments:)

Logs test results to the test log.

``` source
func testLog(
    withFormat format: String!,
    arguments: CVaListPointer
)
```

## Parameters 

`format`  

A string that describes a test result by replacing format indicators with variable data, such as failure details, source code filenames, and line numbers.

`arguments`  

Variable data to replace in the format string, such as failure details, source code filenames, and line numbers.

## See Also

### Logging Test Results

var logFileHandle: FileHandle!

An object to interact with the test log file.

Deprecated

