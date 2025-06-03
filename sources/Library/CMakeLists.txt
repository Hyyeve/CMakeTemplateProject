add_library(Library STATIC)

target_sources(Library PRIVATE
        library.cpp
)

target_sources(Library PUBLIC FILE_SET HEADERS BASE_DIRS ${H_SOURCES_ROOT} FILES
        library.hpp
)

# target link options ..

# target_link_libraries(Library PUBLIC lib)