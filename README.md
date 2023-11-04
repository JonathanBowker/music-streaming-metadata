# Music Streaming Metadata Guide

### Introduction
This guide aims to provide an understanding of the essential metadata required for music streaming services. Metadata helps organize, categorize, and identify music tracks in digital platforms, ensuring accurate tracking, royalty payments, and user satisfaction.

### Core Metadata for Sound Recordings:
- **Recording Title and Sub-Title:** The official name of the track as it should appear on streaming platforms.
- **Recording Artist(s):** The name(s) of the artist(s) who performed the sound recording.
- **Performer and Studio:** The name(s) of the primary performer(s) and the studio where the recording took place.
- **Producer/Personnel Names and Roles:** The individuals responsible for creating and capturing the sound recording and their specific roles (e.g., Producer, Engineer, Mixer).
- **Recording ID (ISRC):** The International Standard Recording Code uniquely identifying the recording.

### Core Metadata for Musical Works:
- **Work Title and Sub-Title:** The name of the composition.
- **Writer Name(s) and Roles:** The name(s) of the writer(s) or composer(s) of the musical work and their contributions (e.g., Lyricist, Composer).
- **Writer IDs (IPI, ISNI):** The Interested Parties Information (IPI) and International Standard Name Identifier (ISNI) numbers for the writers.
- **Work ID (ISWC):** The International Standard Musical Work Code that uniquely identifies the musical work.

### Best Practices
- **Consistency:** Ensure all metadata is consistently applied across all platforms to prevent confusion or misidentification.
- **Accuracy:** Verify all details, especially codes like ISRC and ISWC, to ensure they match the correct recordings and works.
- **Completeness:** Provide as much metadata as possible to give a complete picture of the recording and facilitate better discoverability.

### Schema Definition
Below is a basic JSON schema that defines the structure and data types expected for each field in the metadata:

```json
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "Music Streaming Metadata",
  "type": "object",
  "properties": {
    "SoundRecordingMetadata": {
      "type": "object",
      "properties": {
        "RecordingTitle": { "type": "string" },
        "Subtitle": { "type": "string" },
        "RecordingArtists": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "Name": { "type": "string" },
              "IPN": { "type": "string" },
              "ISNI": { "type": "string" }
            },
            "required": ["Name"]
          }
        },
        "PerformerStudio": { "type": "string" },
        "ProducerPersonnel": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "Name": { "type": "string" },
              "Role": { "type": "string" },
              "IPN": { "type": "string" },
              "ISNI": { "type": "string" }
            },
            "required": ["Name", "Role"]
          }
        },
        "ISRC": { "type": "string", "pattern": "^[A-Z]{2}-[A-Z0-9]{3}-[0-9]{2}-[0-9]{5}$" }
      },
      "required": ["RecordingTitle", "RecordingArtists", "ISRC"]
    },
    "MusicalWorkMetadata": {
      "type": "object",
      "properties": {
        "WorkTitle": { "type": "string" },
        "Subtitle": { "type": "string" },
        "Writers": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "Name": { "type": "string" },
              "Role": { "type": "string" },
              "IPI": { "type": "string" },
              "ISNI": { "type": "string" }
            },
            "required": ["Name"]
          }
        },
        "ISWC": { "type": "string", "pattern": "T-\\d{9}-\\d" }
      },
      "required": ["WorkTitle", "Writers"]
    }
  }
}
```

This is an example:
```
{
  "SoundRecordingMetadata": {
    "RecordingTitle": "Example Title",
    "Subtitle": "Example Subtitle",
    "RecordingArtists": [
      {
        "Name": "Artist Name",
        "IPN": "Artist's IPN if available",
        "ISNI": "Artist's ISNI if available"
      }
    ],
    "PerformerStudio": "Example Studio",
    "ProducerPersonnel": [
      {
        "Name": "Producer Name",
        "Role": "Producer",
        "IPN": "Producer's IPN if available",
        "ISNI": "Producer's ISNI if available"
      }
    ],
    "ISRC": "International Standard Recording Code"
  },
  "MusicalWorkMetadata": {
    "WorkTitle": "Example Work Title",
    "Subtitle": "Example Work Subtitle",
    "Writers": [
      {
        "Name": "Writer Name",
        "Role": "Composer",
        "IPI": "Writer's IPI if available",
        "ISNI": "Writer's ISNI if available"
      }
    ],
    "ISWC": "International Standard Musical Work Code"
  }
}
```

This schema provides a framework for structuring music metadata and can be further customised or extended based on specific requirements or additional metadata fields.

It is essential for anyone using this cookbook to understand that metadata management is an evolving process, and this guide is intended as a starting point. Regular updates and industry consultations are advisable to keep up with best practices and changes in metadata standards.
