SET(LIBMRT_SRC config.c request.c)

ADD_LIBRARY(tdss STATIC ${LIBMRT_SRC})

INSTALL(TARGETS tdss ARCHIVE DESTINATION lib)

INSTALL(FILES tdss_config.h DESTINATION include/libtdss)
