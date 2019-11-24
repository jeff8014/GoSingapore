# Go Singapore

# RTSP Server 실행 방법
 - 설치 참고 사이트(https://imsoftpro.tistory.com/53)
 - `cd gst-rtsp-server/examples/`
 - `test-launch "( rpicamsrc preview=false bitrate=2000000 keyframe-interval=15 ! video/x-h264, width=1080, height=720, framerate=15/1 ! h264parse ! rtph264pay name=pay0 pt=96 )"`
   - 저렇게하면 실행됨. 
   - 설정값 바꾸려면 width, height, framrate같은거 바꿔주심됨
   - 저거 실행하면 아마 127.0.0.1:8554/test 로 열릴꺼임 todo : 0.0.0.0:8554/test로 열어야되지않나?
