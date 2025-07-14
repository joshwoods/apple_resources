

- Matter
- MTROtaSoftwareUpdateRequestorClusterAnnounceOtaProviderParams
-  serverSideProcessingTimeout Deprecated

Instance Property

# serverSideProcessingTimeout

Controls how much time, in seconds, we will allow for the server to process the command.

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
@NSCopying
var serverSideProcessingTimeout: NSNumber? { get set }
```

Deprecated

Please use MTROTASoftwareUpdateRequestorClusterAnnounceOTAProviderParams

## Discussion

The command will then time out if that much time, plus an allowance for retransmits due to network failures, passes.

If nil, the framework will try to select an appropriate timeout value itself.

