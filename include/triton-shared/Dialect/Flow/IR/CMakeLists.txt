set(LLVM_TARGET_DEFINITIONS FlowBase.td)
mlir_tablegen(FlowEnums.h.inc -gen-enum-decls)
mlir_tablegen(FlowEnums.cpp.inc -gen-enum-defs)
add_public_tablegen_target(FlowEnumsGen)

set(LLVM_TARGET_DEFINITIONS FlowOps.td)
mlir_tablegen(FlowOps.h.inc -gen-op-decls)
mlir_tablegen(FlowOps.cpp.inc -gen-op-defs)
add_public_tablegen_target(FlowOpsGen)

set(LLVM_TARGET_DEFINITIONS FlowInterfaces.td)
mlir_tablegen(FlowOpInterfaces.h.inc -gen-op-interface-decls)
mlir_tablegen(FlowOpInterfaces.cpp.inc -gen-op-interface-defs)
mlir_tablegen(FlowTypeInterfaces.h.inc -gen-type-interface-decls)
mlir_tablegen(FlowTypeInterfaces.cpp.inc -gen-type-interface-defs)
add_public_tablegen_target(FlowInterfacesGen)

set(LLVM_TARGET_DEFINITIONS FlowBase.td)
mlir_tablegen(FlowAttrs.h.inc -gen-attrdef-decls --attrdefs-dialect=flow)
mlir_tablegen(FlowAttrs.cpp.inc -gen-attrdef-defs --attrdefs-dialect=flow)
mlir_tablegen(FlowTypes.h.inc -gen-typedef-decls --typedefs-dialect=flow)
mlir_tablegen(FlowTypes.cpp.inc -gen-typedef-defs --typedefs-dialect=flow)
add_public_tablegen_target(FlowTypesGen)
