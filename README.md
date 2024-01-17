# Inhaler

## CMake compilation commands
### Configure and generate build files
cmake.exe --no-warn-unused-cli -DCMAKE_EXPORT_COMPILE_COMMANDS:BOOL=TRUE -Spath-to-your-project-folder -Bpath-to-your-project-folder/build -G build-system
e.g. cmake.exe --no-warn-unused-cli -DCMAKE_EXPORT_COMPILE_COMMANDS:BOOL=TRUE -Spath-to-your-project-folder -Bpath-to-your-project-folder/build -G Ninja
e.g. cmake.exe --no-warn-unused-cli -DCMAKE_EXPORT_COMPILE_COMMANDS:BOOL=TRUE -Spath-to-your-project-folder -Bpath-to-your-project-folder/build -G "NMake Makefiles"
### Build target
cmake.exe --build path-to-your-project-folder/build --target target
e.g. cmake.exe --build path-to-your-project-folder/build --target all
e.g. cmake.exe --build path-to-your-project-folder/build --target clean