project(KemaiCore)

add_library(${PROJECT_NAME})

set(SRCS
        settings.cpp)

set(PUB_HDRS
        include/kemai/settings.h)

set(PRIV_HDRS)

target_sources(${PROJECT_NAME} PRIVATE ${SRCS} ${PRIV_HDRS} ${PUB_HDRS})
target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
target_link_libraries(${PROJECT_NAME} Qt5::Core)
