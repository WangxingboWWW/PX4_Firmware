# PX4 Drone Autopilot 

## Minor changes to increased the stream rate of imu data from MAVROS

## Firmware
  
  * In src/modules/mavlink/mavlink_main.cpp
    * configure_stream_local("HIGHRES_IMU", 400.0f);

## Configuration on QGround

  * MAVLink
    * MAV1_RATE
  * Serial
    * SER_TEL2_BAUD

## Building
  
We build px4_fmu-v5_default(Pixhawk 4) succesfully with gcc-arm-none-eabi-7-2017-q4-major-linux.tar.bz2, don't install gcc-arm-none-eabi with apt-get, and don't download recent releases. 

Links:
* https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads

