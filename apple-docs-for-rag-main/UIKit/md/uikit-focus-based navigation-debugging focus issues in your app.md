

- UIKit
- Focus-based navigation
-  Debugging focus issues in your app 

Article

# Debugging focus issues in your app

Find errors and determine why the next focused item isn’t what you expected.

## Overview

With the use of indirect controls for your tvOS app, it’s imperative that focus works correctly. To help you find focus problems, Apple provides two debugging tools: `UIFocusLoggingEnabled` and UIFocusDebugger.

### Turn on live focus logging

See how the focus engine determines which view is currently in focus by turning on live focus logging. As the user moves focus, the log updates, showing how the new view came into focus.

In your Xcode project, select Edit Scheme and add `-UIFocusLoggingEnabled YES` to the Arguments Passed On Launch section.

On launch, all focus events are logged and displayed in the Xcode console and the Console app. Logs are updated as focus changes in your app.

### Find focus issues using UIFocusDebugger

The UIFocusDebugger class contains several methods to help you find focus issues. You don’t use this class or its methods directly from your code. Instead, during a debugging session, you call the methods of this class from the LLDB debugger command line to obtain information about the state of the focus system. For example, `po UIFocusDebugger.status()` returns the state of the focus engine.

## See Also

### Focus debugging

class UIFocusDebugger

A runtime object for debugging focus-related interactions.

