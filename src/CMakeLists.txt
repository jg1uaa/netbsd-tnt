find_package(Curses)

file(GLOB TNT_SRC
	ax25dump.c
	ax25k.c
	bcast.c
	bcastadd.c
	boxlist.c
	codconv.c
	comp.c
	connect.c
	cookie.c
	crc.c
	display.c
	file.c
	huffman.c
	iface.c
	init.c
	keyboard.c
	log.c
	macro.c
	main.c
	monbox.c
	priv.c
	remote.c
	serial.c
	shell.c
	window.c
	xmon.c
	yapp.c
)
add_executable(tnt ${TNT_SRC})
target_link_libraries(tnt ${Intl_LIBRARY} ${CURSES_LIBRARIES})

project(tntc LANGUAGES C)
file(GLOB TNTC_SRC tntc.c)
add_executable(tntc ${TNTC_SRC})
target_link_libraries(tntc ${Intl_LIBRARY})

add_subdirectory(runprgs)
