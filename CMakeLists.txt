cmake_minimum_required(VERSION 3.5)

project(tetrabiblicu LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(tetrabiblicu main.cpp astro.cpp astro.h
    uelement.h cmemory.h cmemory.cpp uassert.h uhash.h umutex.h umutex.cpp putilimp.h
    gregoimp.h gregoimp.cpp uresimp.h cstring.h cstring.cpp ucln.h uresdata.h uresdata.cpp
    udataswp.h udataswp.cpp ucmndata.h ucmndata.cpp umapfile.h umapfile.cpp uposixdefs.h
    resource.h resource.cpp restrace.h restrace.cpp uarrsort.h uarrsort.cpp
    uinvchar.h uinvchar.cpp ucol_swp.h ucol_swp.cpp utrie.h utrie.cpp utrie2.h utrie2.cpp utrie2_impl.h
    ucol_data.h udatamem.h udatamem.cpp mutex.h)
target_link_libraries(tetrabiblicu /usr/local/lib/libicui18n.so.66 /usr/local/lib/libicuuc.so.66)
