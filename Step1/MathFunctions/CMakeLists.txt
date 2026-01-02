# TODO12: Move all the MathFunctions target commands to this CMakeLists.txt.
#         Ensure that all paths are updated to be relative to this new location.

# TODO6: Add the source and header file located in Step1/MathFunctions to the
#        MathFunctions target, note that the intended way to include the
#        MathFunctions header is:
#          #include <MathFunctions.h>
target_sources(MathFunctions
    PRIVATE
        MathFunctions.cxx 
    
    PUBLIC
        FILE_SET mathHeaders
    TYPE HEADERS 
    BASE_DIRS
    FILES
        MathFunctions.h
)
