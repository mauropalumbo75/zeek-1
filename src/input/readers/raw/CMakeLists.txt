
include(ZeekPlugin)

include_directories(BEFORE ${CMAKE_CURRENT_SOURCE_DIR} ${CMAKE_CURRENT_BINARY_DIR})

zeek_plugin_begin(Zeek RawReader)
zeek_plugin_cc(Raw.cc Plugin.cc)
zeek_plugin_bif(raw.bif)
zeek_plugin_end()
