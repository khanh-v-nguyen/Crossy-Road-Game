cmake_minimum_required(VERSION 3.17)
project(SFML_Template)

set(CMAKE_CXX_STANDARD 14)

add_executable(SFML_Template main.cpp Player.h Player.cpp Obstacles.cpp Obstacles.h StartingScreen.h StartingScreen.cpp ListItem.h ListItem.cpp List.h List.cpp Position.h Position.cpp CarRow.h CarRow.cpp ObstacleType.h Map.h Map.cpp MouseEvents.h MouseEvents.cpp CrossyRoad.h CrossyRoad.cpp bootlegMain.cpp GameEnum.h WinLose.h WinLose.cpp States.h States.cpp statesEnum.h)

target_link_libraries(SFML_Template sfml-graphics sfml-audio)

find_package(SFML 2.5 COMPONENTS graphics audio REQUIRED)