# Streaming a video through FFMPEG and RTSP.

## Workflow:-
1. Start the RTSP Server in the AWS or any cloud instance which will now act as a server.
2. We are going to use [RTSP Server Library](https://github.com/aler9/rtsp-simple-server) as our RTSP server. We can start this server by storing this library as a code in S3 Bucket and obtaining the same in our instance through wget command in linux.
3. Start the rtsp server using the below command in the terminal of the same directory.
```
./rtsp-simple-server
```
4. Now note the IP address of the instance and make the change in the rtspserver variable.
5. Now run the python code. Your camera will be taken as input and the stream starts.
6. You can view the same in any device by mentioning the IP address of the instance in the RTSP section. 