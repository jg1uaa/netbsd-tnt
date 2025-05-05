project(tnt-help LANGUAGES C)
file(GLOB HELP_SRC help.c)
add_executable(tnt-help ${HELP_SRC})
target_link_libraries(tnt-help ${Intl_LIBRARY})

project(tnt-info LANGUAGES C)
file(GLOB INFO_SRC info.c)
add_executable(tnt-info ${INFO_SRC})
target_link_libraries(tnt-info ${Intl_LIBRARY})

project(tnt-logcall LANGUAGES C)
file(GLOB LOGCALL_SRC logcall.c)
add_executable(tnt-logcall ${LOGCALL_SRC})
target_link_libraries(tnt-logcall ${Intl_LIBRARY})
