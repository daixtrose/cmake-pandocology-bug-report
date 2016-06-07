# cmake "C:\Program Files (x86)\GnuWin32\bin\make.exe"
# using https://github.com/jeetsukumaran/cmake-pandocology

cmake_minimum_required(VERSION 3.2)
set(CMAKE_VERBOSE_MAKEFILE ON)

LIST(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake/Modules/cmake-pandocology")
INCLUDE(pandocology)

project(paper NONE)

set(RUNTIME_OUTPUT_DIRECTORY Sections CACHE PATH "Build directory" FORCE)
set(LIBRARY_OUTPUT_DIRECTORY Sections CACHE PATH "Library directory" FORCE)


add_document(
    test.tex
    SOURCES ../Markdown/test.md
	PANDOC_DIRECTIVES -f markdown_github -t latex 
    #PRODUCT_DIRECTORY "./Sections"
)