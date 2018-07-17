set(LLVM_LINK_COMPONENTS support)

add_clang_library(clangTidyBtcModule
  BtcTidyModule.cpp
  DerivedFromSharableStackProhibitoionCheck.cpp

  LINK_LIBS
  clangAST
  clangASTMatchers
  clangBasic
  clangLex
  clangTidy
  clangTidyUtils
  )
