cmake_policy(SET CMP0037 OLD)	# to enable filename "help"
project(help LANGUAGES C)
file(GLOB HELP_SRC help.c)
add_executable(help ${HELP_SRC})
target_link_libraries(help ${Intl_LIBRARY})

project(info LANGUAGES C)
file(GLOB INFO_SRC info.c)
add_executable(info ${INFO_SRC})
target_link_libraries(info ${Intl_LIBRARY})

project(logcall LANGUAGES C)
file(GLOB LOGCALL_SRC logcall.c)
add_executable(logcall ${LOGCALL_SRC})
target_link_libraries(logcall ${Intl_LIBRARY})
