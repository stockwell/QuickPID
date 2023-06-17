set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

file(GLOB_RECURSE SOURCES src/*.cpp)

idf_component_register(SRCS ${SOURCES}
                       INCLUDE_DIRS src
                       REQUIRES main esp_timer)
