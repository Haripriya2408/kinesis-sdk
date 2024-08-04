sudo apt-get install -y git pkg-config cmake m4 build-essential \
    gstreamer1.0 gstreamer1.0-plugins-base gstreamer1.0-plugins-good \
    gstreamer1.0-plugins-ugly gstreamer1.0-libav libgstreamer1.0-dev \
    libgstreamer-plugins-base1.0-dev
AKIAZQ3DTNSU5QVI5IEQamu
05xhJnk5weeroVCGJpTzRJV4T/Uw8hQZV/vMmxrRhari

































sudo apt-get install gstreamer1.0-tools gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-bad gstreamer1.0-plugins-ugly gstreamer1.0-libav gstreamer1.0-doc gstreamer1.0-dev


pkg-config --version
cmake --version
m4 --version
gst-launch-1.0 --version




















sudo apt-get update && sudo apt-get install -y pkg-config cmake m4 build-essential gstreamer1.0-tools gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-ugly gstreamer1.0-plugins-bad libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev
cmake .. -DBUILD_GSTREAMER_PLUGIN=ON -DBUILD_JNI=TRUE -- Found Log4cplus: /home/lubuntu/Desktop/amazon-kinesis-video-streams-producer-sdk-cpp/open-source/local/lib/liblog4cplus.so  
CMake Error at /usr/share/cmake-3.28/Modules/FindPackageHandleStandardArgs.cmake:230 (message):                                             
  Could NOT find JNI (missing: JAVA_INCLUDE_PATH JAVA_INCLUDE_PATH2 AWT JVM)                                                                
Call Stack (most recent call first):                                  
  /usr/share/cmake-3.28/Modules/FindPackageHandleStandardArgs.cmake:600 (_FPHSA_FAILURE_MESSAGE)                                            
  /usr/share/cmake-3.28/Modules/FindJNI.cmake:589 (find_package_handle_standard_args)                                                       
  CMakeLists.txt:204 (find_package)   
aws_secret_key





sudo apt-get update && sudo apt-get install -y pkg-config cmake m4 build-essential gstreamer1.0-tools gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-ugly gstreamer1.0-plugins-bad libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev default-jdk


echo 'export JAVA_HOME=/usr/lib/jvm/default-java' >> ~/.bashrc
echo 'export PATH=$JAVA_HOME/bin:$PATH' >> ~/.bashrc



ubuntu@lubuntu:~$ gst-launch-1.0 v4l2src do-timestamp=TRUE device=/dev/video0 ! videoconvert ! video/x-raw,format=I420,width=640,height=480,framerate=30/1 ! x264enc  bframes=0 key-int-max=45 bitrate=500 ! video/x-h264,stream-format=avc,alignment=au,profile=baseline ! kvssink stream-name="cameravisionvideostream" storage-size=512 access-key="aws_access_id" secret-key="aws_secret_key" aws-region="ap-south-1" 
Command 'gst-launch-1.0' is available in the following places
 * /bin/gst-launch-1.0
 * /usr/bin/gst-launch-1.0
The command could not be located because '/bin:/usr/bin' is not included in the PATH environment variable.
gst-launch-1.0: command not found



source ~/.bashrc

cmake .. -DBUILD_GSTREAMER_PLUGIN=ON -DBUILD_JNI=TRUE



https://github.com/awsdocs/Aws-Kinesis-Video-Documentation/blob/master/doc_source/examples-gstreamer-plugin.md

