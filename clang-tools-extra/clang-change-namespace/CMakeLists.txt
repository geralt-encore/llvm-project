set(LLVM_LINK_COMPONENTS
  FrontendOpenMP
  Support
  )

add_clang_library(clangChangeNamespace
  ChangeNamespace.cpp

  LINK_LIBS
  clangAST
  clangASTMatchers
  clangBasic
  clangFormat
  clangFrontend
  clangLex
  clangSerialization
  clangTooling
  clangToolingCore
  )

add_subdirectory(tool)
