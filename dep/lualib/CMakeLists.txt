#
# Copyright (C) 2010 - 2014 Eluna Lua Engine <http://emudevs.com/>
# This program is free software licensed under GPL version 3
# Please see the included DOCS/LICENSE.md for more information
#

file(GLOB sources src/*.h)

set(lua51_STAT_SRCS
  ${sources}
)

include_directories(
  ${CMAKE_CURRENT_SOURCE_DIR}/src
)

add_library(lua51 STATIC ${lua51_STAT_SRCS})
set_target_properties(lua51 PROPERTIES LINKER_LANGUAGE C)
