

- Application Services
- Speech Synthesis Manager
-  SpeechErrorInfo 

Structure

# SpeechErrorInfo

Defines a speech error information structure.

macOS 10.0+

``` source
struct SpeechErrorInfo
```

## Overview

By calling the GetSpeechInfo function with the `soErrors` selector, you can obtain a speech error information structure, which shows what Speech Synthesis Manager errors occurred while processing a text buffer on a given speech channel.

Speech error information structures never include errors that are returned by Speech Synthesis Manager functions. Instead, they reflect only errors encountered directly in the processing of text, and, in particular, in the processing of commands embedded within text.

The speech error information structure keeps track of only the most recent error and the first error that occurred after the previous call to the `GetSpeechInfo` function with the `soErrors` selector. If your application needs to keep track of all errors, then you should install an error callback function, SpeechErrorProcPtr.

## Topics

### Initializers

init()

init(count: Int16, oldest: OSErr, oldPos: Int, newest: OSErr, newPos: Int)

### Instance Properties

var count: Int16

The number of errors that have occurred in processing the current text buffer since the last call to the `GetSpeechInfo` function with the `soErrors` selector. Of these errors, you can find information about only the first and last error that occurred.

var newPos: Int

The character position within the text buffer being processed of the most recent error.

var newest: OSErr

The error code of the most recent error.

var oldPos: Int

The character position within the text buffer being processed of the first error that occurred after the previous call to the `GetSpeechInfo` function with the `soErrors` selector.

var oldest: OSErr

The error code of the first error that occurred after the previous call to the `GetSpeechInfo` function with the `soErrors` selector.

