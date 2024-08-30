add_triton_library(UtilIR
  ClosureOpUtils.cpp
  UtilAttrs.cpp
  UtilDialect.cpp
  UtilOpFolders.cpp
  UtilOps.cpp
  UtilTypes.cpp

  DEPENDS
  UtilAttrsGen
  UtilInterfacesGen
  UtilOpsGen
  UtilTypesGen
  LLVMSupport
  MLIRAffineDialect
  MLIRArithDialect
  MLIRCastInterfaces
  MLIRControlFlowDialect
  MLIRControlFlowInterfaces
  MLIRFuncDialect
  MLIRFunctionInterfaces
  MLIRIR
  MLIRInferTypeOpInterface
  MLIRMemRefDialect
  MLIRParser
  MLIRSideEffectInterfaces
  MLIRSupport
  MLIRTensorDialect
  MLIRTransformUtils
  MLIRTransforms
  MLIRViewLikeInterface

  LINK_LIBS PUBLIC
  MLIRIR
  )
