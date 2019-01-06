cmake_minimum_required(VERSION 2.8)

set(CMAKE_CXX_FLAGS "--std=c++0x -Wall -pedantic")
include_directories(sokoban/include/)

set(SOURCES 
		sokoban/src/main.cpp
		sokoban/src/GraphicEngine.cpp
		sokoban/src/Player.cpp
		sokoban/src/Button.cpp
		sokoban/src/LogicManager.cpp
	)

add_executable(game ${SOURCES})
target_link_libraries(game SDL opengl32 glu32 glut32 SDL_image)


