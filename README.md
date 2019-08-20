# streaming_server_built
Server will reading config file for initialize
Config filename: config.ss 
# Syntax
## Unique header
  - Type: Client/Proxy/Server (Only Proxy is completed)
  - Location: path to storage folder
## Special header
  - --: Using as a scope to separate streams
## Common header
  - Stream: stream url
  - Name: Stream name (using for API)
  - Interval: record interval (second)
## Other
  - //, #: this line will be count as comment
## Example
Config example:\
///////////////////////////////////////\
Type: Proxy\
Location: /mnt/data/\
//Stream 1\
--\
Stream: rtsp://user:password@127.0.0.1:8554/Streaming/Channels/101/\
Name: Test1\
Interval: 10\
//Stream 2
-- \
Stream: rtsp://user:password@127.0.0.1:8554/Streaming/Channels/102/\
Name: Test2\
Interval: 10
