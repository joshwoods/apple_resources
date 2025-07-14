

- os
- Logging
-  Viewing Log Messages 

Article

# Viewing Log Messages

Use various tools to retrieve log information.

## Overview

The unified log system stores log messages in a binary compressed format, deferring much of the work to turn them into human-readable text messages. Using a binary format allows the log system to store more messages and reduces the overhead of logging data. However, this means you can’t read and parse the log files directly; you need to use tools to convert the log messages into a binary format. Depending on which tool you use, this conversion might be done while your app is running, or later, after the app has already exited.

Here are some of the tools you can use to read log data:

- The Console app provides a graphical user interface for reading and sorting through log data.

- Use the `log` tool to retrieve log messages from a command-line.

- When you run your app in Xcode with the debugger attached, Xcode automatically displays logged messages. Similarly, you can use launch Instruments from inside Xcode to record and analyze signposts created by your app.

- Use the OSLog framework to access logged messages programmatically.

## See Also

### Essentials

Generating Log Messages from Your Code

Record useful debugging and analysis information, and include dynamic content in your messages.

Customizing Logging Behavior While Debugging

Control which log events are recorded.

