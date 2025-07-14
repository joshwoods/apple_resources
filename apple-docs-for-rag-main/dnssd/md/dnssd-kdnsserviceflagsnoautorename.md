

- dnssd
-  kDNSServiceFlagsNoAutoRename 

Global Variable

# kDNSServiceFlagsNoAutoRename

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var kDNSServiceFlagsNoAutoRename: UInt32 { get }
```

## Discussion

Flag for specifying renaming behavior on name conflict when registering non-shared records. By default, name conflicts are automatically handled by renaming the service. NoAutoRename overrides this behavior - with this flag set, name conflicts will result in a callback. The NoAutorename flag is only valid if a name is explicitly specified when registering a service (i.e. the default name is not used.)

