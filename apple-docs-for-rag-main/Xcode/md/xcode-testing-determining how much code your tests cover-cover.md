

- Xcode
- Testing
-  Determining how much code your tests cover 

Article

# Determining how much code your tests cover

Use code coverage to focus new test development on areas that lack adequate testing.

## Overview

By implementing code coverage, you can visualize and measure how much of your code you are actually testing. Use it during development to identify areas that your tests are missing. Although achieving a high level of coverage is an excellent goal, code coverage alone doesn’t ensure that your tests are doing their job and are robust enough for unexpected behaviors. Be sure to pair high code coverage with well-written tests.

Code coverage can answer:

- What code is actually running when you perform your tests?

- What parts of your code aren’t you testing?

- Have you written enough tests to ensure that you’re checking all of your code?

### Enable code coverage in your test plan

Code coverage is a testing option you can configure for your test plans. When you enable code coverage, the build system instructs the code to gather coverage data based on the frequency that it calls methods and functions. The code coverage option can collect data to report on tests of correctness and of performance, whether unit tests or UI tests.

Note

Code coverage data collection impacts your code’s performance. Even if the impact is significant, it is also linear, so results between two runs with code coverage enabled remain comparable. However, consider its impact when critically evaluating the performance of routines in your tests.

You enable code coverage in the Configurations pane of your test plan using the following steps:

1.  Open a test plan from the Project navigator or the scheme editor. For more information on creating a test plan, see Improving code assessment by organizing tests into test plans.

2.  Click the Configurations tab.

3.  Select a specific configuration, or select Shared Settings to enable testing across all configurations.

4.  Scroll down to the Code Coverage section.

5.  Click the value for Code Coverage and select the “Gather coverage for” checkbox on the popover.

6.  Use the options from the pop-up menu to select targets to collect the information from.

### Examine code coverage results

After completing a test run, Xcode uses the coverage data to create a report in the Coverage pane of the Report navigator. The coverage report shows summary information about the test run, a listing of source files and functions within the files, and the coverage percentage for each.

The source editor shows counts for each line of code in the file, and highlights code that didn’t execute. It highlights areas of code that need coverage rather than areas that have coverage.

For example, positioning the pointer over the `Calculator.input(_:)` method in the coverage report above shows a button that takes you to the annotated source code.

The coverage annotation appears on the right and shows the number of times that the test executed a particular part of the code. You can hover over areas with red highlights to identify code your test didn’t cover.

According to the counts in the screenshot above, the test frequently called the `Calculator.input(_:)` method. However, there are sections of the method that the test didn’t call. This report data indicates an opportunity to write a test for a missing condition to ensure that the error handling works the way you intend.

Note

Swift Testing and XCTest support ways to identify a test to skip or a test you expect to fail due to known issue. Code coverage metrics do not include skipped tests but they do include tests that run marked with known issues or expected failures. Consider this when evaluating code coverage and attempt to resolve issues as soon as possible.

## See Also

### Test development

Adding tests to your Xcode project

Include test targets that build code to test the logic in your functions, check for integration issues, automate UI workflows, and measure performance.

Updating your existing codebase to accommodate unit tests

Remove coupling between components to increase test coverage and reliability.

Improving code assessment by organizing tests into test plans

Control the information you receive from your tests at different stages in the software engineering process by creating and configuring test plans.

