# CMakeList.txt: проект CMake для Matrix_extra; включите исходный код и определения,
# укажите здесь логику для конкретного проекта.
#

# Добавьте источник в исполняемый файл этого проекта.
add_executable (Matrix_extra "Matrix_extra.cpp" "Matrix_extra.h" "Matrix.h" "Column.h" "Matrix.cpp" "Column.cpp" "String.cpp" "String.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET Matrix_extra PROPERTY CXX_STANDARD 20)
endif()

# TODO: Добавьте тесты и целевые объекты, если это необходимо.
