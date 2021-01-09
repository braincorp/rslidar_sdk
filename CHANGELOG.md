# Changelog

## v1.3.1 - 2021-01-08

### Changed
- Set CMake COMPILE_METHOD variable to CATKIN (since we still use catkin)
- Changed definition of PROJECT_PATH in CMake (so we find the config file in the right place)
- Copied package_ros1.xml as package.xml (see README.md, doubt we'll ever move to ROS2)
- Changed config lidar_type to RSBP

### Removed
- Commented out building with protobuf in CMake (for now, due to mismatched libprotobuf .so in build container and sandbox)
- Removed package_ros[1|2].xml

## v1.3.0 - 2020-11-10

### Added

- Add multi-cast support
- Add saved_by_rows argument
- Add different point types( XYZI & XYZIRT)

### Changed

- Update driver core, please refer to CHANGELOG in rs_driver for details
- Update some documents
- Change angle_path argument to hiding parameter

### Removed

- Remove RSAUTO for lidar type
- Remove device_ip argument



## v1.2.1 - 2020-09-04

### Fixed

- Fix bug in driver core, please refer to changelog in rs_driver for details.


## v1.2.0 - 2020-09-01

### Added
- Add camera software trigger (base on target angle)

### Changed
- Update driver core, please refer to changelog in rs_driver for details
- Update the compiler version from C++11 to C++14


## v1.1.0 - 2020-07-01

### Added

- Add ROS2 support

### Changed
- Replace while loop with cv.wait
- Update the vector copy part 
- Update the program structure

### Removed
- Remove some unused variables in message struct

## v1.0.0 - 2020-06-01

### Added

- New program structure

- Support ROS & Protobuf-UDP functions

  
