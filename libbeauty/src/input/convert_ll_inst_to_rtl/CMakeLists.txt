set(the_description "Input ll_inst_to_rtl")
#libbeauty_define_module(beauty_ll_inst_to_rtl)
add_library(beauty_ll_inst_to_rtl dis.c)
set_target_properties(beauty_ll_inst_to_rtl PROPERTIES SOVERSION 1)
set_target_properties(beauty_ll_inst_to_rtl PROPERTIES VERSION "1.0.0")
target_link_libraries(beauty_ll_inst_to_rtl )
target_include_directories(beauty_ll_inst_to_rtl PRIVATE "${libbeauty_INCLUDE_DIRS}")
install (TARGETS beauty_ll_inst_to_rtl DESTINATION lib/beauty)
