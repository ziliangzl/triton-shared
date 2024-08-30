add_triton_library(FlowIR
  FlowOps.cpp
  FlowDialect.cpp
  FlowTypes.cpp
  FlowOpFolders.cpp

  DEPENDS
  FlowEnumsGen
  FlowTypesGen
  FlowOpsGen
  FlowInterfacesGen

  LINK_LIBS PUBLIC
  UtilIR
  MLIRIR
  )
