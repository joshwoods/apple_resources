

- XCTest
-  Test Execution and Observation 

API Collection

# Test Execution and Observation

Observe, introspect, and customize the test execution flow.

## Topics

### Test Failures

Capture test failures with `XCTIssue` and related classes that associate source code locations and call stacks with failures.

struct XCTIssue

An object that represents a test failure, and includes source code call stacks for test reporting and investigation.

class XCTIssueReference

An object that represents a test failure, and includes source code call stacks for test reporting and investigation.

class XCTMutableIssue

A mutable object that represents a test failure, and includes source code call stacks for test reporting and investigation.

class XCTSourceCodeContext

An object that contains call stack and source code location details to provide context for a point of execution in a test.

class XCTSourceCodeFrame

An object that represents a single frame in a call stack that supports retrieval of symbol information for the address.

class XCTSourceCodeLocation

An object that contains a file URL and line number that represents a distinct location in source code.

class XCTSourceCodeSymbolInfo

An object that contains symbolication information for a specified frame in a call stack.

### Test Runs

class XCTestCaseRun

An object that collects information about a specific execution of a test case.

class XCTestSuiteRun

An object that collects information about a specific execution of a test suite.

class XCTestRun

A base class for collecting information about a specific execution of a test.

### Test Observation

protocol XCTestObservation

A protocol that defines methods the test runner calls in response to significant events during test runs.

class XCTestObservationCenter

Provides information about the progress of test runs to registered observers.

### Test Suites

class XCTestSuite

A collection of test cases to manage as a test suite.

