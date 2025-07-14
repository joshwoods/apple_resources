

- watchOS apps
-  Setting up tests for your watchOS app 

Article

# Setting up tests for your watchOS app

Configure your watch-only project with unit tests and user interface tests.

## Overview

Xcode offers unit and user interface tests to use while building your watchOS app. Add them to your project to confirm that your features work as expected, prevent performance regressions, and validate user interaction flows.

### Add a test target to the project

Add a unit test or UI test target to your existing watch-only watchOS Xcode project by choosing File \> New \> Target to open the template selection dialog. Alternatively, select the project in the Project navigator, select the General tab, and click the Add a Target button (+) at the bottom of the Targets area.

Xcode presents the template selection dialog. Select watchOS, and then select the watchOS UI Testing Bundle or the watchOS Unit Testing Bundle option in the Test section, and click Next.

Specify a name for the test target, and then choose the WatchKit Extension option as the target if you’re adding unit tests, or the WatchKit App option if you’re adding UI tests.

Xcode adds the target and template files to your project, and creates a new scheme to run your tests. Select the new scheme, named \[*Project Name*\] `WatchKit ExtensionTests`, from the list of schemes in Xcode’s toolbar, and choose Edit Scheme.

Confirm the selected executable is \[*Project Name*\] `WatchKit App.app`. If not, choose it and click Close.

### Make the extension code visible in unit tests

When you add a unit test file to your test target, your watch extension code isn’t visible to your tests by default. Add an `@testable import` declaration at the top of your test file, specifying your watch extension name, to make your extension code testable.

### Switch schemes to run tests

If you try to run your tests before switching to the new test scheme, Xcode lets you know that the current scheme isn’t set up for testing.

Click Cancel and select the new test scheme from the list of schemes in Xcode’s toolbar, and choose Product \> Test to run your tests.

