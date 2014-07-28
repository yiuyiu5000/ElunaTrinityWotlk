#
# Copyright (C) 2010 - 2014 Eluna Lua Engine <http://emudevs.com/>
# This program is free software licensed under GPL version 3
# Please see the included DOCS/LICENSE.md for more information
#

file(GLOB sources src/*.c)

set(lua_STAT_SRCS
  ${sources}
)

include_directories(
  ${CMAKE_CURRENT_SOURCE_DIR}/src
)

add_library(lua51 SHARED ${lua_STAT_SRCS})
