# Radio Station Recorder

A bash script for recording audio streams from online radio stations. This tool allows you to easily manage and record multiple radio stations through a simple command-line interface.

## Features

- Record audio streams from online radio stations
- Configure multiple radio stations
- List available stations
- View recording history
- Simple command-line interface

## Prerequisites

- Bash shell
- wget
- A Unix-like operating system (Linux, macOS)

## Installation

1. Clone this repository or download the script files
2. Make the script executable:
3. Create a configuration file named `radio_stations.conf` with your radio stations

## Configuration

Create a `radio_stations.conf` file in the same directory as the script with the following format:

```
StationName=http://stream-url.com/stream
AnotherStation=http://another-stream-url.com/stream
```

Example:

```
Radio1=http://stream.radio1.com/live
JazzFM=http://stream.jazzfm.com/live
```

## Usage

### Basic Commands

```bash
# Show help
./recording_script -h
./recording_script --help

# List available stations
./recording_script -l
./recording_script --list

# Start recording a station (where N is the station ID)
./recording_script -r N
./recording_script --record N

# Show all recordings
./recording_script -s
./recording_script --show

# Show recordings for a specific station
./recording_script -s N
./recording_script --show N
```

### Examples

```bash
# List all configured stations
./recording_script --list

# Start recording station ID 0
./recording_script --record 0

# View all recordings
./recording_script --show
```

## Output Files

Recordings are saved in the following format:

```
recording_STATIONNAME_YYYYMMDD_HHMMSS.mp3
```

## Credits

ASCII art generated using [ASCII Generator](https://ascii-generator.site/t/)
