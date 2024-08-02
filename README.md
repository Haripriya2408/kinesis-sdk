sudo apt-get update && sudo apt-get install -y pkg-config cmake m4 build-essential gstreamer1.0-tools gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-ugly gstreamer1.0-plugins-bad libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev
cmake .. -DBUILD_GSTREAMER_PLUGIN=ON -DBUILD_JNI=TRUE -- Found Log4cplus: /home/lubuntu/Desktop/amazon-kinesis-video-streams-producer-sdk-cpp/open-source/local/lib/liblog4cplus.so  
CMake Error at /usr/share/cmake-3.28/Modules/FindPackageHandleStandardArgs.cmake:230 (message):                                             
  Could NOT find JNI (missing: JAVA_INCLUDE_PATH JAVA_INCLUDE_PATH2 AWT JVM)                                                                
Call Stack (most recent call first):                                  
  /usr/share/cmake-3.28/Modules/FindPackageHandleStandardArgs.cmake:600 (_FPHSA_FAILURE_MESSAGE)                                            
  /usr/share/cmake-3.28/Modules/FindJNI.cmake:589 (find_package_handle_standard_args)                                                       
  CMakeLists.txt:204 (find_package)   
05xhJnk5weeroVCGJpTzRJV4T/Uw8hQZV/vMmxrR





sudo apt-get update && sudo apt-get install -y pkg-config cmake m4 build-essential gstreamer1.0-tools gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-ugly gstreamer1.0-plugins-bad libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev default-jdk


echo 'export JAVA_HOME=/usr/lib/jvm/default-java' >> ~/.bashrc
echo 'export PATH=$JAVA_HOME/bin:$PATH' >> ~/.bashrc


source ~/.bashrc

cmake .. -DBUILD_GSTREAMER_PLUGIN=ON -DBUILD_JNI=TRUE



https://github.com/awsdocs/Aws-Kinesis-Video-Documentation/blob/master/doc_source/examples-gstreamer-plugin.md

