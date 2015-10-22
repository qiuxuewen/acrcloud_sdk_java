# acrcloud_sdk_java
create  "ACRCloud Fingerprint" by Audio/Video file, and use "ACRCloud Fingerprint" to recognize metainfos by "ACRCloud webapi".

# Overview
This java SDK can recognize ACRCloud by most of audio/video file.<br>
>>>>Audio: mp3, wav, m4a, flac, aac, amr, ape, ogg ...<br>
>>>>Video: mp4, mkv, wmv, flv, ts, avi ...

# Functions
Introduction all API.
## src/com/acrcloud/utils/ACRCloudRecognizer.java
```java
      public String recognizeByFile(String filePath, int startSeconds)
      /**
      *
      *  recognize by file path of (Audio/Video file)
      *          Audio: mp3, wav, m4a, flac, aac, amr, ape, ogg ...
      *          Video: mp4, mkv, wmv, flv, ts, avi ...
      *
      *  @param filePath query file path
      *  @param startSeconds skip (startSeconds) seconds from from the beginning of (filePath)
      *
      *  @return result
      *
      **/
    
      public String recognizeByFileBuffer(byte[] fileBuffer, int fileBufferLen, int startSeconds)
      /**
      *
      *  recognize by buffer of (Audio/Video file)
      *          Audio: mp3, wav, m4a, flac, aac, amr, ape, ogg ...
      *          Video: mp4, mkv, wmv, flv, ts, avi ...
      *
      *  @param fileBuffer query buffer
      *  @param fileBufferLen the length of fileBufferLen
      *  @param startSeconds skip (startSeconds) seconds from from the beginning of fileBuffer
      *
      *  @return result
      *
      **/
    
      public String recognize(byte[] wavAudioBuffer, int wavAudioBufferLen)
      /**
      *
      *  recognize by wav audio buffer(RIFF (little-endian) data, WAVE audio, Microsoft PCM, 16 bit, mono 8000 Hz)
      *
      *  @param wavAudioBuffer query audio buffer
      *  @param wavAudioBufferLen the length of wavAudioBuffer
      *
      *  @return result
      *
      **/
```
