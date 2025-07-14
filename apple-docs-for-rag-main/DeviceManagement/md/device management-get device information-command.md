

- Device Management
-  Get Device Information 

Web Service Endpoint

# Get Device Information

Get detailed information about a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#DeviceInformationCommand
```

## HTTP Body

DeviceInformationCommand

The command to query a device for specific information.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

DeviceInformationResponse

`OK`

A response from the device after it processes the command to get detailed information.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS, Shared iPad                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | Special case (see subkeys)             |

### Example Request and Response

- Request
- Response

```

    Command

        Queries

            UDID
            Languages
            Locales
            DeviceID
            OrganizationInfo
            LastCloudBackupDate
            AwaitingConfiguration
            MDMOptions
            iTunesStoreAccountIsActive
            iTunesStoreAccountHash
            DeviceName
            OSVersion
            BuildVersion
            ModelName
            Model
            ProductName
            SerialNumber
            DeviceCapacity
            AvailableDeviceCapacity
            BatteryLevel
            CellularTechnology
            ICCID
            BluetoothMAC
            WiFiMAC
            EthernetMACs
            CurrentCarrierNetwork
            SubscriberCarrierNetwork
            CurrentMCC
            CurrentMNC
            SubscriberMCC
            SubscriberMNC
            SIMMCC
            SIMMNC
            SIMCarrierNetwork
            CarrierSettingsVersion
            PhoneNumber
            DataRoamingEnabled
            VoiceRoamingEnabled
            PersonalHotspotEnabled
            IsRoaming
            IMEI
            MEID
            ModemFirmwareVersion
            IsSupervised
            IsDeviceLocatorServiceEnabled
            IsActivationLockEnabled
            IsDoNotDisturbInEffect
            EASDeviceIdentifier
            IsCloudBackupEnabled
            OSUpdateSettings
            LocalHostName
            HostName
            CatalogURL
            IsDefaultCatalog
            PreviousScanDate
            PreviousScanResult
            PerformPeriodicCheck
            AutomaticCheckEnabled
            BackgroundDownloadEnabled
            AutomaticAppInstallationEnabled
            AutomaticOSInstallationEnabled
            AutomaticSecurityUpdatesEnabled
            OSUpdateSettings
            LocalHostName
            HostName
            IsMultiUser
            IsMDMLostModeEnabled
            MaximumResidentUsers
            PushToken
            DiagnosticSubmissionEnabled
            AppAnalyticsEnabled
            IsNetworkTethered
            ServiceSubscriptions

        RequestType
        DeviceInformation

    CommandUUID
    0001_DeviceInformation

```

```

    CommandUUID
    0001_DeviceInformation
    QueryResponses

        AppAnalyticsEnabled

        AvailableDeviceCapacity
        225.2413330078125
        AwaitingConfiguration

        BatteryLevel
        1.0
        BluetoothMAC
        58:fe:f7:70:9d:9e
        BuildVersion
        17A576
        CarrierSettingsVersion
        38.0
        CellularTechnology
        3
        CurrentMCC
        311
        CurrentMNC
        480
        DataRoamingEnabled

        DeviceCapacity
        230.26551818847656
        DeviceName
        iPhone
        DiagnosticSubmissionEnabled

        EASDeviceIdentifier
        V2UVOT7J157L7C1FLLSAABSOV4
        ICCID
        8901 0030 0000 0336 1196
        IMEI
        35 735005 003432 4
        IsActivationLockEnabled

        IsCloudBackupEnabled

        IsDeviceLocatorServiceEnabled

        IsDoNotDisturbInEffect

        IsMDMLostModeEnabled

        IsMultiUser

        IsNetworkTethered

        IsRoaming

        IsSupervised

        MDMOptions

        MEID
        35745019114431
        Model
        993-31388LL
        ModelName
        iPhone
        ModemFirmwareVersion
        2.01.08
        OSVersion
        13.0
        PersonalHotspotEnabled

        PhoneNumber

        ProductName
        iPhone11,8
        SerialNumber
        C7CX706CKWTK
        ServiceSubscriptions

                CarrierSettingsVersion
                41.7.19
                CurrentCarrierNetwork

                CurrentMCC
                310
                CurrentMNC
                260
                ICCID
                8901 0030 0000 0336 1196
                IMEI
                35 734009 035404 0
                IsDataPreferred

                IsRoaming

                IsVoicePreferred

                Label
                Primary
                LabelID
                EB91134A-B155-4DAB-9D35-CB2EAF82615D
                MEID
                35735009002431
                PhoneNumber
                +12018675309
                Slot
                CTSubscriptionSlotOne

                CarrierSettingsVersion
                41.7.46
                CurrentCarrierNetwork
                AT&amp;T
                CurrentMCC
                310
                CurrentMNC
                410
                EID
                89049032004008882600004821436874
                ICCID
                6905 4911 1205 0650 3488
                IMEI
                35 309418 464558 9
                IsDataPreferred

                IsRoaming

                IsVoicePreferred

                Label
                Secondary
                LabelID
                FDG4225C-L9OY-89BM-JF38-36JR4JOL76B3
                MEID
                35745008005631
                PhoneNumber
                +14152739164
                Slot
                CTSubscriptionSlotTwo

        SubscriberCarrierNetwork
        ExampleCarrier
        SubscriberMCC
        001
        SubscriberMNC
        01
        UDID
        00008020-000915083C80012E
        VoiceRoamingEnabled

        WiFiMAC
        58:fe:f5:80:29:f3
        iTunesStoreAccountIsActive

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object DeviceInformationCommand

The command to query a device for specific information.

object DeviceInformationResponse

A response from the device after it processes the command to get detailed information.

## See Also

### Device Details

List the Installed Apps

Get a list of the installed apps on a device.

Release Device from Await Configuration

Inform the device that it can allow the user to continue in Setup Assistant.

User Configured Command

Informs the device that it can continue past Setup Assistant and finish login.

List the Installed Restrictions

Get a list of restrictions on the device.

