add_subdirectory(cuda)
add_subdirectory(function)
add_subdirectory(utils)
add_subdirectory(testing)
add_subdirectory(math)
add_subdirectory(parameter)
add_subdirectory(gserver)
add_subdirectory(pserver)
add_subdirectory(trainer)
add_subdirectory(scripts)
add_subdirectory(string)

if(Boost_FOUND)
  add_subdirectory(memory)
  add_subdirectory(platform)
  add_subdirectory(framework)
  add_subdirectory(operators)
  add_subdirectory(pybind)
endif()

if(WITH_C_API)
    add_subdirectory(capi)
endif()

if(WITH_SWIG_PY)
  add_subdirectory(api)
endif()
