#add_subdirectory("app")
#add_subdirectory("setup")

if(WIN32)
  add_subdirectory("ovrcore")
  add_subdirectory("svchook")
  add_subdirectory("appfw")
else()
  message(WARNING "Building ovrcore/svchook/appfw projects for non-Win32 platforms is not supported.")
  message(WARNING "You can ignore these warnings if you're building app/setup projects for Linux.")
endif()
