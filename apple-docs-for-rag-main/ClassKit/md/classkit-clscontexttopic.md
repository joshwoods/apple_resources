

- ClassKit
-  CLSContextTopic 

Structure

# CLSContextTopic

The areas of study to which contexts may relate.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
struct CLSContextTopic
```

## Mentioned in 

Building missing contexts

## Discussion

After you initialize a context, you can assign it a topic by setting its topic property. Doing so helps teachers browsing your app’s content to understand what your app offers.

## Topics

### Context Topics

static let artsAndMusic: CLSContextTopic

Arts and music.

static let computerScienceAndEngineering: CLSContextTopic

Computer science and engineering.

static let healthAndFitness: CLSContextTopic

Health and fitness.

static let literacyAndWriting: CLSContextTopic

Literacy and writing.

static let math: CLSContextTopic

Mathematics.

static let science: CLSContextTopic

Science.

static let socialScience: CLSContextTopic

Social science.

static let worldLanguage: CLSContextTopic

Language acquisition.

### Initializing a Topic

init(rawValue: String)

Initializes a context topic.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing context presentation

var displayOrder: Int

The position of a context relative to its siblings.

var topic: CLSContextTopic?

The area of study to which a context relates.

