message("visiting src")

file(GLOB_RECURSE VehicleDetectionLib_source src/*)
add_executable(VehicleDetectionLib ${VehicleDetectionLib_source})

find_package(OpenCV REQUIRED)
target_link_libraries(VehicleDetectionLib ${OpenCV_LIBS})

