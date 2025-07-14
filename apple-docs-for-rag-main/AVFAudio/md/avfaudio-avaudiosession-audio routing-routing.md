

- AVFAudio
- AVAudioSession
-  Audio routing 

API Collection

# Audio routing

Inspect and configure audio routes, ports, and data sources.

## Topics

### Inspecting the current route

var currentRoute: AVAudioSessionRouteDescription

A description of the current audio route’s input and output ports.

class AVAudioSessionRouteDescription

An object that describes the input and output ports associated with a session’s audio route.

class AVAudioSessionPortDescription

Information about the capabilities of the port and the hardware channels it supports.

class let routeChangeNotification: NSNotification.Name

A notification the system posts when its audio route changes.

### Configuring inputs

var isInputAvailable: Bool

A Boolean value that indicates whether an audio input path is available.

var availableInputs: [AVAudioSessionPortDescription]?

An array of input ports available for audio routing.

var preferredInput: AVAudioSessionPortDescription?

The preferred input port for audio routing.

func setPreferredInput(AVAudioSessionPortDescription?) throws

Sets the preferred input port for audio routing.

var inputDataSource: AVAudioSessionDataSourceDescription?

The currently selected input data source.

var inputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available data sources for the audio session’s current input port.

func setInputDataSource(AVAudioSessionDataSourceDescription?) throws

Selects a data source for the audio session’s current input port.

### Configuring outputs

var outputDataSources: [AVAudioSessionDataSourceDescription]?

An array of available output data sources for the current audio route.

var outputDataSource: AVAudioSessionDataSourceDescription?

The currently selected output data source.

func setOutputDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the output data source for an audio session.

class AVAudioSessionDataSourceDescription

An object that defines a data source for an audio input or output, giving information such as the source’s name, location, and orientation.

func overrideOutputAudioPort(AVAudioSession.PortOverride) throws

Temporarily changes the current audio route.

