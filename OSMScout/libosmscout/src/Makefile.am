AM_CPPFLAGS = $(LIB_CXXFLAGS) \
              $(OPENMP_CXXFLAGS) \
              $(SIMD_FLAGS) \
              $(MARISA_CFLAGS) \
              -DOSMSCOUTDLL -I$(top_srcdir)/include

lib_LTLIBRARIES = libosmscout.la

libosmscout_la_LDFLAGS = -no-undefined \
                         $(OPENMP_CXXFLAGS) \
                         $(MARISA_LIBS)

libosmscout_la_SOURCES= osmscout/util/Breaker.cpp \
                        osmscout/util/Cache.cpp \
                        osmscout/util/Color.cpp \
                        osmscout/util/File.cpp \
                        osmscout/util/FileScanner.cpp \
                        osmscout/util/FileWriter.cpp \
                        osmscout/util/GeoBox.cpp \
                        osmscout/util/Geometry.cpp \
                        osmscout/util/Logger.cpp \
                        osmscout/util/Magnification.cpp \
                        osmscout/util/NodeUseMap.cpp \
                        osmscout/util/Number.cpp \
                        osmscout/util/NumberSet.cpp \
                        osmscout/util/Parser.cpp \
                        osmscout/util/Progress.cpp \
                        osmscout/util/Projection.cpp \
                        osmscout/util/Reference.cpp \
                        osmscout/util/StopClock.cpp \
                        osmscout/util/String.cpp \
                        osmscout/util/Tiling.cpp \
                        osmscout/util/Transformation.cpp \
                        osmscout/Types.cpp \
                        osmscout/TypeConfig.cpp \
                        osmscout/TypeFeatures.cpp \
                        osmscout/TypeSet.cpp \
                        osmscout/ost/Scanner.cpp \
                        osmscout/ost/Parser.cpp \
                        osmscout/GroundTile.cpp \
                        osmscout/Intersection.cpp \
                        osmscout/Location.cpp \
                        osmscout/Coord.cpp \
                        osmscout/GeoCoord.cpp \
                        osmscout/Pixel.cpp \
                        osmscout/Area.cpp \
                        osmscout/Node.cpp \
                        osmscout/Path.cpp \
                        osmscout/Point.cpp \
                        osmscout/Tag.cpp \
                        osmscout/TurnRestriction.cpp \
                        osmscout/Way.cpp \
                        osmscout/ObjectRef.cpp \
                        osmscout/NumericIndex.cpp \
                        osmscout/CoordDataFile.cpp \
                        osmscout/NodeDataFile.cpp \
                        osmscout/AreaAreaIndex.cpp \
                        osmscout/AreaNodeIndex.cpp \
                        osmscout/AreaWayIndex.cpp \
                        osmscout/LocationIndex.cpp \
                        osmscout/OptimizeAreasLowZoom.cpp \
                        osmscout/OptimizeWaysLowZoom.cpp \
                        osmscout/WaterIndex.cpp \
                        osmscout/Route.cpp \
                        osmscout/RouteData.cpp \
                        osmscout/RouteNode.cpp \
                        osmscout/RoutePostprocessor.cpp \
                        osmscout/RoutingProfile.cpp \
                        osmscout/Database.cpp \
                        osmscout/DebugDatabase.cpp \
                        osmscout/SRTM.cpp \
                        osmscout/LocationService.cpp \
                        osmscout/POIService.cpp \
                        osmscout/RoutingService.cpp                         

if OSMSCOUT_HAVE_SSE2
libosmscout_la_SOURCES+=osmscout/system/SSEMath.cpp
endif

if OSMSCOUT_HAVE_LIB_MARISA
libosmscout_la_SOURCES+=osmscout/TextSearchIndex.cpp
endif
