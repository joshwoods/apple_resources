

- Matter
- MTROtaSoftwareUpdateProviderClusterQueryImageParams
-  timedInvokeTimeoutMs Deprecated

Instance Property

# timedInvokeTimeoutMs

Controls whether the command is a timed command (using Timed Invoke).

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
@NSCopying
var timedInvokeTimeoutMs: NSNumber? { get set }
```

Deprecated

Please use MTROTASoftwareUpdateProviderClusterQueryImageParams

## Discussion

If nil (the default value), a regular invoke is done for commands that do not require a timed invoke and a timed invoke with some default timed request timeout is done for commands that require a timed invoke.

If not nil, a timed invoke is done, with the provided value used as the timed request timeout. The value should be chosen small enough to provide the desired security properties but large enough that it will allow a round-trip from the sever to the client (for the status response and actual invoke request) within the timeout window.

