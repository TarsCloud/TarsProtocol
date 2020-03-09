set(OUT_DEPENDS_LIST)

complice_tars(OUT_DEPENDS_LIST)

add_custom_target(FRAMEWORK-PROTOCOL ALL DEPENDS ${OUT_DEPENDS_LIST})

set(FRAMEWORKPROTOCOLS
        AdminReg.tars
        AdminReg.h
        MonitorQuery.tars
        MonitorQuery.h
        Node.tars
        Node.h
        NodeDescriptor.tars
        NodeDescriptor.h
        Patch.tars
        Patch.h
        Registry.tars
        Registry.h
        RegistryDescriptor.tars
        RegistryDescriptor.h)

INSTALL(FILES ${FRAMEWORKPROTOCOLS} DESTINATION  include/framework)
