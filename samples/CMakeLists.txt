
if (POLICY CMP0074)
  cmake_policy(SET CMP0074 NEW)
endif()


INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR})
INCLUDE_DIRECTORIES(${CMAKE_CURRENT_BINARY_DIR})


SET(LIBS ${LIBS} curve_fit)


ADD_EXECUTABLE(fit-demo fit_demo.cpp)
TARGET_LINK_LIBRARIES(fit-demo 
	${LIBS})
	
	
#INSTALL(TARGETS stereo_demo DESTINATION bin)

