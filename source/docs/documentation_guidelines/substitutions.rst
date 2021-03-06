.. _substitutions:

*************
Substitutions
*************

.. contents::
   :local:

Usage
=====

To easier the use of icons in QGIS manuals, replacements are defined
for each icon in :file:`/source/substitutions.txt` file at `QGIS-Documentation repository
<https://github.com/qgis/QGIS-Documentation>`_ and some of these substitutions
are listed below.
Thus, when you want to use an icon from QGIS application in the documentation
there is a big chance that there is already a substitution that can/should be used.

If no replacement exists:

* check the documentation repository whether the icon is available in
  :file:`/resources/en/docs/common` folder. If no image, then you need to find and
  copy the icon image file from `QGIS repository <https://github.com/qgis/QGIS>`_
  (often under https://github.com/qgis/QGIS/tree/master/images/themes/default folder)
  and paste (in ``.png`` format) under :file:`/static/common` folder.
  For convenience and update, it's advised to keep filename when possible.
* create the reference to the substitution in the :file:`/source/substitutions.txt`
  file following the example below. The replacement text should be in camelCase:

::

  .. |splitLayer| image:: /static/common/split_layer.png
     :width: 1.5em

* run the :file:`scripts\find_set_subst.py` script to update the substitution
  definitions in the rst files and include the new substitution(s).
* (optional) add the reference to the icon and its substitution to the list below.

Common Substitutions
====================

Below are given some icons and their substitution to use when writing documentation.
Can be used/found in many places in manuals.

Platform Icons
..............

==========  ===============  ==========  =============== 
Icon        Substitution     Icon        Substitution
==========  ===============  ==========  =============== 
|kde|       ``|kde|``        |nix|       ``|nix|``
|osx|       ``|osx|``        |win|       ``|win|``
==========  ===============  ==========  =============== 



Menu Items
..........

=======================  =========================  =====================  =========================
Icon                     Substitution               Icon                   Substitution
=======================  =========================  =====================  =========================
|checkbox|               ``|checkbox|``             |unchecked|            ``|unchecked|``
|radioButtonOn|          ``|radioButtonOn|``        |radioButtonOff|       ``|radioButtonOff|``
|selectNumber|           ``|selectNumber|``         |selectString|         ``|selectString|``
|browseButton|           ``|browseButton|``         |slider|               ``|slider|``
|selectColor|            ``|selectColor|``          |inputText|            ``|inputText|``
|tab|                    ``|tab|``                  |degrees|              ``|degrees|``
=======================  =========================  =====================  =========================


Toolbar Button Icons
====================

Manage Layers and overview
..........................

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|addOgrLayer|                   ``|addOgrLayer|``                   |addDb2Layer|                   ``|addDb2Layer|``
|addRasterLayer|                ``|addRasterLayer|``                |addMssqlLayer|                 ``|addMssqlLayer|``
|addDelimitedTextLayer|         ``|addDelimitedTextLayer|``         |addSpatiaLiteLayer|            ``|addSpatiaLiteLayer|``
|addPostgisLayer|               ``|addPostgisLayer|``               |addOracleLayer|                ``|addOracleLayer|``
|addAfsLayer|                   ``|addAfsLayer|``                   |addAmsLayer|                   ``|addAmsLayer|``
|virtualLayer|                  ``|virtualLayer|``                  |wms|                           ``|wms|``
|wcs|                           ``|wcs|``                           |wfs|                           ``|wfs|``
|newVectorLayer|                ``|newVectorLayer|``                |newSpatiaLiteLayer|            ``|newSpatiaLiteLayer|``
|newGeoPackageLayer|            ``|newGeoPackageLayer|``            |createMemory|                  ``|createMemory|``
|dbManager|                     ``|dbManager|``                     |gdal|                          ``|gdal|``
|inOverview|                    ``|inOverview|``                    |addAllToOverview|              ``|addAllToOverview|``
|removeAllOVerview|             ``|removeAllOVerview|``             |removeLayer|                   ``|removeLayer|``
|showAllLayers|                 ``|showAllLayers|``                 |hideAllLayers|                 ``|hideAllLayers|``
|showMapTheme|                  ``|showMapTheme|``                  |showSelectedLayers|            ``|showSelectedLayers|``
|hideSelectedLayers|            ``|hideSelectedLayers|``            |hideDeselectedLayers|          ``|hideDeselectedLayers|``
|addLayer|                      ``|addLayer|``                      |zip|                           ``|zip|``
==============================  ==================================  ==============================  ==================================

File
....

=======================  ===========================  =======================  ===========================
Icon                     Substitution                 Icon                     Substitution
=======================  ===========================  =======================  ===========================
|fileNew|                ``|fileNew|``                |fileOpen|               ``|fileOpen|``
|fileSave|               ``|fileSave|``               |fileSaveAs|             ``|fileSaveAs|``
|fileExit|               ``|fileExit|``               \                        \
=======================  ===========================  =======================  ===========================

Edit
....

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|undo|                          ``|undo|``                          |redo|                          ``|redo|``
|editCopy|                      ``|editCopy|``                      |editPaste|                     ``|editPaste|``
|editCut|                       ``|editCut|``                       |saveEdits|                     ``|saveEdits|``
==============================  ==================================  ==============================  ==================================

Identity result
...............

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|expandTree|                    ``|expandTree|``                    |collapseTree|                  ``|collapseTree|``
|expandNewTree|                 ``|expandNewTree|``                 |propertyItem|                  ``|propertyItem|``
|deselectAll|                   ``|deselectAll|``                   |editCopy|                      ``|editCopy|``
|filePrint|                     ``|filePrint|``                     |propertiesWidget|              ``|propertiesWidget|``
==============================  ==================================  ==============================  ==================================


Digitizing and Advanced Digitizing
..................................

============================  =================================  =============================  ================================
Icon                          Substitution                       Icon                           Substitution
============================  =================================  =============================  ================================
|cad|                         ``|cad|``                          |cadConstruction|              ``|cadConstruction|``
|cadParallel|                 ``|cadParallel|``                  |cadPerpendicular|             ``|cadPerpendicular|``
|toggleEditing|               ``|toggleEditing|``                |allEdits|                     ``|allEdits|``
|tracing|                     ``|tracing|``                      |snapping|                     ``|snapping|``
|capturePoint|                ``|capturePoint|``                 |capturePolygon|               ``|capturePolygon|``
|captureLine|                 ``|captureLine|``                  \                              \
|circularStringCurvePoint|    ``|circularStringCurvePoint|``     |circularStringRadius|         ``|circularStringRadius|``
|nodeTool|                    ``|nodeTool|``                     |deleteSelected|               ``|deleteSelected|``
|moveFeature|                 ``|moveFeature|``                  |rotateFeature|                ``|rotateFeature|``
|simplifyFeatures|            ``|simplifyFeatures|``             |reshape|                      ``|reshape|``
|addRing|                     ``|addRing|``                      |addPart|                      ``|addPart|``
|fillRing|                    ``|fillRing|``                     \                              \
|deleteRing|                  ``|deleteRing|``                   |deletePart|                   ``|deletePart|``
|mergeFeatures|               ``|mergeFeatures|``                |mergeFeatAttributes|          ``|mergeFeatAttributes|``
|splitFeatures|               ``|splitFeatures|``                |splitParts|                   ``|splitParts|``
|offsetPointSymbols|          ``|offsetPointSymbols|``           |rotatePointSymbols|           ``|rotatePointSymbols|``
|offsetCurve|                 ``|offsetCurve|``                  \                              \
============================  =================================  =============================  ================================


Map Navigation and attributes
.............................

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|pan|                           ``|pan|``                           |panToSelected|                 ``|panToSelected|``
|zoomIn|                        ``|zoomIn|``                        |zoomOut|                       ``|zoomOut|``
|zoomActual|                    ``|zoomActual|``                    |zoomFullExtent|                ``|zoomFullExtent|``
|zoomToLayer|                   ``|zoomToLayer|``                   |zoomToSelected|                ``|zoomToSelected|``
|zoomLast|                      ``|zoomLast|``                      |zoomNext|                      ``|zoomNext|``
|touch|                         ``|touch|``                         |draw|                          ``|draw|``
|identify|                      ``|identify|``                      |mapTips|                       ``|mapTips|``
|showBookmarks|                 ``|showBookmarks|``                 |newBookmark|                   ``|newBookmark|``
|measure|                       ``|measure|``                       |measureArea|                   ``|measureArea|``
|measureAngle|                  ``|measureAngle|``                  |newMap|                        ``|newMap|``
==============================  ==================================  ==============================  ==================================

Selection and Expressions
.........................

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|selectRectangle|               ``|selectRectangle|``               |selectPolygon|                 ``|selectPolygon|``
|selectFreehand|                ``|selectFreehand|``                |selectRadius|                  ``|selectRadius|``
|selectAll|                     ``|selectAll|``                     |deselectAll|                   ``|deselectAll|``
|invertSelection|               ``|invertSelection|``               |expressionSelect|              ``|expressionSelect|``
|selectAllTree|                 ``|selectAllTree|``                 |select|                        ``|select|``
|formSelect|                    ``|formSelect|``                    |dataDefined|                   ``|dataDefined|``
|expression|                    ``|expression|``                    |dataDefineOn|                  ``|dataDefineOn|``
|dataDefineExpressionOn|        ``|dataDefineExpressionOn|``        |dataDefineError|               ``|dataDefineError|``
|dataDefineExpressionError|     ``|dataDefineExpressionError|``     |filter|                        ``|filter|``
|expressionFilter|              ``|expressionFilter|``              |filterMap|                     ``|filterMap|``
==============================  ==================================  ==============================  ==================================


Labels and Diagrams
...................

=======================  ===========================  =======================  ===========================
Icon                     Substitution                 Icon                     Substitution
=======================  ===========================  =======================  ===========================
|labeling|               ``|labeling|``               |labelingNone|           ``|labelingNone|``
|labelingRuleBased|      ``|labelingRuleBased|``      |labelingObstacle|       ``|labelingObstacle|``
|piechart|               ``|piechart|``               |diagramNone|            ``|diagramNone|``
|text|                   ``|text|``                   |histogram|              ``|histogram|``
|annotation|             ``|annotation|``             |textAnnotation|         ``|textAnnotation|``
|formAnnotation|         ``|formAnnotation|``         |htmlAnnotation|         ``|htmlAnnotation|``
|svgAnnotation|          ``|svgAnnotation|``          |autoPlacement|          ``|autoPlacement|``
=======================  ===========================  =======================  ===========================

Help
....

=======================  ===========================  =======================  ==================================
Icon                     Substitution                 Icon                     Substitution
=======================  ===========================  =======================  ==================================
|helpContents|           ``|helpContents|``           |qgisHomePage|           ``|qgisHomePage|``
|checkQgisVersion|       ``|checkQgisVersion|``       |helpAbout|              ``|helpAbout|``
|helpSponsors|           ``|helpSponsors|``           |contextHelp|            ``|contextHelp|``
=======================  ===========================  =======================  ==================================

Colors
......

=======================  ===========================  =======================  ===========================
Icon                     Substitution                 Icon                     Substitution
=======================  ===========================  =======================  ===========================
|colorBox|               ``|colorBox|``               |colorPicker|            ``|colorPicker|``
|colorSwatches|          ``|colorSwatches|``          |colorWheel|             ``|colorWheel|``
=======================  ===========================  =======================  ===========================


Other basic icons
=================

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|arrowDown|                     ``|arrowDown|``                     |arrowUp|                       ``|arrowUp|``
|arrowLeft|                     ``|arrowLeft|``                     |arrowRight|                    ``|arrowRight|``
|signPlus|                      ``|signPlus|``                      |signMinus|                     ``|signMinus|``
|projectProperties|             ``|projectProperties|``             |options|                       ``|options|``
|copyrightLabel|                ``|copyrightLabel|``                |northArrow|                    ``|northArrow|``
|scaleBar|                      ``|scaleBar|``                      |locale|                        ``|locale|``
|gpsImporter|                   ``|gpsImporter|``                   |gpsTrackBarChart|              ``|gpsTrackBarChart|``
|gpsTrackPolarChart|            ``|gpsTrackPolarChart|``            |tracking|                      ``|tracking|``
|folder|                        ``|folder|``                        |extents|                       ``|extents|``
|settings|                      ``|settings|``                      \                               \
==============================  ==================================  ==============================  ==================================


Attribute Table
===============

============================ ===============================  =======================  ===========================
Icon                         Substitution                     Icon                     Substitution
============================ ===============================  =======================  ===========================
|openTable|                  ``|openTable|``                  |selectedToTop|          ``|selectedToTop|``
|selectAll|                  ``|selectAll|``                  |invertSelection|        ``|invertSelection|``
|panToSelected|              ``|panToSelected|``              |zoomToSelected|         ``|zoomToSelected|``
|copySelected|               ``|copySelected|``               |editPaste|              ``|editPaste|``
|expressionSelect|           ``|expressionSelect|``           |deleteSelected|         ``|deleteSelected|``
|newAttribute|               ``|newAttribute|``               |deleteAttribute|        ``|deleteAttribute|``
|newTableRow|                ``|newTableRow|``                |calculateField|         ``|calculateField|``
|draw|                       ``|draw|``                       |formView|               ``|formView|``
|conditionalFormatting|      ``|conditionalFormatting|``      |multiEdit|              ``|multiEdit|``
|attributes|                 ``|attributes|``                 \                        \
============================ ===============================  =======================  ===========================


Projections and Georeferencer
=============================

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|geographic|                    ``|geographic|``                    |crs|                           ``|crs|``
|customProjection|              ``|customProjection|``              |setProjection|                 ``|setProjection|``
|projectionDisabled|            ``|projectionDisabled|``            |projectionEnabled|             ``|projectionEnabled|``
|georeferencer|                 ``|georeferencer|``                 |pencil|                        ``|pencil|``
|linkQGisToGeoref|              ``|linkQGisToGeoref|``              |linkGeorefToQGis|              ``|linkGeorefToQGis|``
|coordinateCapture|             ``|coordinateCapture|``             |startGeoref|                   ``|startGeoref|``
==============================  ==================================  ==============================  ==================================


Print Layout
============

=======================  ===========================  =======================  ===========================
Icon                     Substitution                 Icon                     Substitution
=======================  ===========================  =======================  ===========================
|newLayout|              ``|newLayout|``              |layoutManager|          ``|layoutManager|``
|duplicateLayout|        ``|duplicateLayout|``        \                        \
|atlasSettings|          ``|atlasSettings|``          |atlas|                  ``|atlas|``
|filePrint|              ``|filePrint|``              |saveMapAsImage|         ``|saveMapAsImage|``
|saveAsSVG|              ``|saveAsSVG|``              |saveAsPDF|              ``|saveAsPDF|``
|addArrow|               ``|addArrow|``               |addBasicShape|          ``|addBasicShape|``
|addNodesShape|          ``|addNodesShape|``          |editNodesShape|         ``|editNodesShape|``
|addMap|                 ``|addMap|``                 |addLegend|              ``|addLegend|``
|addHtml|                ``|addHtml|``                |addTable|               ``|addTable|``
|label|                  ``|label|``                  |scaleBar|               ``|scaleBar|``
|select|                 ``|select|``                 |moveItemContent|        ``|moveItemContent|``
|raiseItems|             ``|raiseItems|``             |lowerItems|             ``|lowerItems|``
|moveItemsToTop|         ``|moveItemsToTop|``         |moveItemsToBottom|      ``|moveItemsToBottom|``
|alignLeft|              ``|alignLeft|``              |alignRight|             ``|alignRight|``
|alignHCenter|           ``|alignHCenter|``           |alignVCenter|           ``|alignVCenter|``
|alignTop|               ``|alignTop|``               |alignBottom|            ``|alignBottom|``
|locked|                 ``|locked|``                 |unlocked|               ``|unlocked|``
|lockedRepeat|           ``|lockedRepeat|``           |groupItems|             ``|groupItems|``
=======================  ===========================  =======================  ===========================

Layer Properties
================

==================================  ======================================  =============================  ================================
Icon                                Substitution                            Icon                           Substitution
==================================  ======================================  =============================  ================================
|symbology|                         ``|symbology|``                         |labeling|                     ``|labeling|``
|sourceFields|                      ``|sourceFields|``                      |general|                      ``|general|``
|metadata|                          ``|metadata|``                          |action|                       ``|action|``
|mapTips|                           ``|mapTips|``                           |rendering|                    ``|rendering|``
|join|                              ``|join|``                              |diagram|                      ``|diagram|``
|legend|                            ``|legend|``                            |dependencies|                 ``|dependencies|``
|3d|                                ``|3d|``                                |system|                       ``|system|``
|editMetadata|                      ``|editMetadata|``                      |overlay|                      ``|overlay|``
|history|                           ``|history|``                           |stylePreset|                  ``|stylePreset|``
|singleSymbol|                      ``|singleSymbol|``                      |nullSymbol|                   ``|nullSymbol|``
|graduatedSymbol|                   ``|graduatedSymbol|``                   |categorizedSymbol|            ``|categorizedSymbol|``
|25dSymbol|                         ``|25dSymbol|``                         |ruleBasedSymbol|              ``|ruleBasedSymbol|``
|invertedSymbol|                    ``|invertedSymbol|``                    |heatmapSymbol|                ``|heatmapSymbol|``
|pointDisplacementSymbol|           ``|pointDisplacementSymbol|``           |pointClusterSymbol|           ``|pointClusterSymbol|``
|sum|                               ``|sum|``                               |sort|                         ``|sort|``
|paintEffects|                      ``|paintEffects|``                      |mapIdentification|            ``|mapIdentification|``
==================================  ======================================  =============================  ================================


Plugins
=======

Vector Menu
...........

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|matrix|                        ``|matrix|``                        |unique|                        ``|unique|``
|sumLines|                      ``|sumLines|``                      |sumPoints|                     ``|sumPoints|``
|basicStatistics|               ``|basicStatistics|``               |neighbor|                      ``|neighbor|``
|mean|                          ``|mean|``                          |intersections|                 ``|intersections|``
|randomSelection|               ``|randomSelection|``               |subSelection|                  ``|subSelection|``
|randomPoints|                  ``|randomPoints|``                  \                                \
|regularPoints|                 ``|regularPoints|``                 |vectorGrid|                    ``|vectorGrid|``
|selectLocation|                ``|selectLocation|``                |layerExtent|                   ``|layerExtent|``
|convexHull|                    ``|convexHull|``                    |buffer|                        ``|buffer|``
|intersect|                     ``|intersect|``                     |union|                         ``|union|``
|symDifference|                 ``|symDifference|``                 |clip|                          ``|clip|``
|difference|                    ``|difference|``                    |dissolve|                      ``|dissolve|``
|checkGeometry|                 ``|checkGeometry|``                 |exportGeometry|                ``|exportGeometry|``
|delaunay|                      ``|delaunay|``                      |centroids|                     ``|centroids|``
|simplify|                      ``|simplify|``                      |joinLocation|                  ``|joinLocation|``
|multiToSingle|                 ``|multiToSingle|``                 |singleToMulti|                 ``|singleToMulti|``
|toLines|                       ``|toLines|``                       |extractNodes|                  ``|extractNodes|``
|exportProjection|              ``|exportProjection|``              |defineProjection|              ``|defineProjection|``
|splitLayer|                    ``|splitLayer|``                    |mergeShapes|                   ``|mergeShapes|``
==============================  ==================================  ==============================  ==================================

Raster Menu
...........

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|fullCumulativeStretch|         ``|fullCumulativeStretch|``         |fullHistogramStretch|          ``|fullHistogramStretch|``
|showRasterCalculator|          ``|showRasterCalculator|``          |rasterStats|                   ``|rasterStats|``
|rasterInterpolate|             ``|rasterInterpolate|``             |rasterInfo|                    ``|rasterInfo|``
|rasterTerrain|                 ``|rasterTerrain|``                 |heatmap|                       ``|heatmap|``
==============================  ==================================  ==============================  ==================================

Various Core Plugins
....................

Standard provided with basic install, but not loaded with initial install

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|showPluginManager|             ``|showPluginManager|``             |pluginInstaller|               ``|pluginInstaller|``
|installPluginFromZip|          ``|installPluginFromZip|``          \                               \
|offlineEditingCopy|            ``|offlineEditingCopy|``            |offlineEditingSync|            ``|offlineEditingSync|``
|plugin|                        ``|plugin|``                        |interpolation|                 ``|interpolation|``
|delimitedText|                 ``|delimitedText|``                 \                               \
|gdalScript|                    ``|gdalScript|``                    |dxf2shpConverter|              ``|dxf2shpConverter|``
|metasearch|                    ``|metasearch|``
|geometryChecker|               ``|geometryChecker|``               |geometrySnapper|               ``|geometrySnapper|``
|topologyChecker|               ``|topologyChecker|``               |oracleRaster|                  ``|oracleRaster|``
==============================  ==================================  ==============================  ==================================

Grass integration
.................

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|grass|                         ``|grass|``                         \                               \
|grassTools|                    ``|grassTools|``                    |grassNewMapset|                ``|grassNewMapset|``
|grassOpenMapset|               ``|grassOpenMapset|``               |grassCloseMapset|              ``|grassCloseMapset|``
|grassRegion|                   ``|grassRegion|``                   |grassSetRegion|                ``|grassSetRegion|``
==============================  ==================================  ==============================  ==================================

OpenStreetMap
.............

=============================  =================================  =============================  ==================================
Icon                            Substitution                      Icon                           Substitution
=============================  =================================  =============================  ==================================
|osmLoad|                      ``|osmLoad|``                      |osmDownload|                  ``|osmDownload|``
|osmFeatureManager|            ``|osmFeatureManager|``            |osmIdentify|                  ``|osmIdentify|``
|osmImport|                    ``|osmImport|``                    |osmSave|                      ``|osmSave|``
|osmCreatePoint|               ``|osmCreatePoint|``               |osmCreateLine|                ``|osmCreateLine|``
|osmCreatePolygon|             ``|osmCreatePolygon|``             \                              \
|osmMove|                      ``|osmMove|``                      |osmRemoveFeat|                ``|osmRemoveFeat|``
|osmCreateRelation|            ``|osmCreateRelation|``            |osmAddRelation|               ``|osmAddRelation|``
|osmEditRelation|              ``|osmEditRelation|``              |osmGenerateTags|              ``|osmGenerateTags|``
|osmQuestionMark|              ``|osmQuestionMark|``              \                              \
=============================  =================================  =============================  ==================================

eVis plugin
...........

==============================  ==================================  ==============================  ==================================
Icon                            Substitution                        Icon                            Substitution
==============================  ==================================  ==============================  ==================================
|eventBrowser|                  ``|eventBrowser|``                  |eventId|                       ``|eventId|``
|evisConnect|                   ``|evisConnect|``                   |evisFile|                      ``|evisFile|``
==============================  ==================================  ==============================  ==================================


.. Substitutions definitions - AVOID EDITING PAST THIS LINE
   This will be automatically updated by the find_set_subst.py script.
   If you need to create a new substitution manually,
   please add it also to the substitutions.txt file in the
   source folder.

.. |25dSymbol| image:: /static/common/renderer25dSymbol.png
   :width: 1.5em
.. |3d| image:: /static/common/3d.png
   :width: 1.5em
.. |action| image:: /static/common/action.png
   :width: 2em
.. |addAfsLayer| image:: /static/common/mActionAddAfsLayer.png
   :width: 1.5em
.. |addAllToOverview| image:: /static/common/mActionAddAllToOverview.png
   :width: 1.5em
.. |addAmsLayer| image:: /static/common/mActionAddAmsLayer.png
   :width: 1.5em
.. |addArrow| image:: /static/common/mActionAddArrow.png
   :width: 1.5em
.. |addBasicShape| image:: /static/common/mActionAddBasicShape.png
   :width: 1.5em
.. |addDb2Layer| image:: /static/common/mActionAddDb2Layer.png
   :width: 1.5em
.. |addDelimitedTextLayer| image:: /static/common/mActionAddDelimitedTextLayer.png
   :width: 1.5em
.. |addHtml| image:: /static/common/mActionAddHtml.png
   :width: 1.5em
.. |addLayer| image:: /static/common/mActionAddLayer.png
   :width: 1.5em
.. |addLegend| image:: /static/common/mActionAddLegend.png
   :width: 1.5em
.. |addMap| image:: /static/common/mActionAddMap.png
   :width: 1.5em
.. |addMssqlLayer| image:: /static/common/mActionAddMssqlLayer.png
   :width: 1.5em
.. |addNodesShape| image:: /static/common/mActionAddNodesShape.png
   :width: 1.5em
.. |addOgrLayer| image:: /static/common/mActionAddOgrLayer.png
   :width: 1.5em
.. |addOracleLayer| image:: /static/common/mActionAddOracleLayer.png
   :width: 1.5em
.. |addPart| image:: /static/common/mActionAddPart.png
   :width: 1.5em
.. |addPostgisLayer| image:: /static/common/mActionAddPostgisLayer.png
   :width: 1.5em
.. |addRasterLayer| image:: /static/common/mActionAddRasterLayer.png
   :width: 1.5em
.. |addRing| image:: /static/common/mActionAddRing.png
   :width: 2em
.. |addSpatiaLiteLayer| image:: /static/common/mActionAddSpatiaLiteLayer.png
   :width: 1.5em
.. |addTable| image:: /static/common/mActionAddTable.png
   :width: 1.5em
.. |alignBottom| image:: /static/common/mActionAlignBottom.png
   :width: 1.5em
.. |alignHCenter| image:: /static/common/mActionAlignHCenter.png
   :width: 1.5em
.. |alignLeft| image:: /static/common/mActionAlignLeft.png
   :width: 1.5em
.. |alignRight| image:: /static/common/mActionAlignRight.png
   :width: 1.5em
.. |alignTop| image:: /static/common/mActionAlignTop.png
   :width: 1.5em
.. |alignVCenter| image:: /static/common/mActionAlignVCenter.png
   :width: 1.5em
.. |allEdits| image:: /static/common/mActionAllEdits.png
   :width: 1.5em
.. |annotation| image:: /static/common/mActionAnnotation.png
   :width: 1.5em
.. |arrowDown| image:: /static/common/mActionArrowDown.png
   :width: 1.5em
.. |arrowLeft| image:: /static/common/mActionArrowLeft.png
   :width: 1.5em
.. |arrowRight| image:: /static/common/mActionArrowRight.png
   :width: 1.5em
.. |arrowUp| image:: /static/common/mActionArrowUp.png
   :width: 1.5em
.. |atlas| image:: /static/common/mIconAtlas.png
   :width: 1.5em
.. |atlasSettings| image:: /static/common/mActionAtlasSettings.png
   :width: 1.5em
.. |attributes| image:: /static/common/attributes.png
   :width: 2em
.. |autoPlacement| image:: /static/common/mIconAutoPlacementSettings.png
   :width: 1.5em
.. |basicStatistics| image:: /static/common/basic_statistics.png
   :width: 1.5em
.. |browseButton| image:: /static/common/browsebutton.png
   :width: 2.3em
.. |buffer| image:: /static/common/buffer.png
   :width: 1.5em
.. |cad| image:: /static/common/cad.png
   :width: 1.5em
.. |cadConstruction| image:: /static/common/cad_construction.png
   :width: 1.5em
.. |cadParallel| image:: /static/common/cad_parallel.png
   :width: 1.5em
.. |cadPerpendicular| image:: /static/common/cad_perpendicular.png
   :width: 1.5em
.. |calculateField| image:: /static/common/mActionCalculateField.png
   :width: 1.5em
.. |captureLine| image:: /static/common/mActionCaptureLine.png
   :width: 1.5em
.. |capturePoint| image:: /static/common/mActionCapturePoint.png
   :width: 1.5em
.. |capturePolygon| image:: /static/common/mActionCapturePolygon.png
   :width: 1.5em
.. |categorizedSymbol| image:: /static/common/rendererCategorizedSymbol.png
   :width: 1.5em
.. |centroids| image:: /static/common/centroids.png
   :width: 1.5em
.. |checkGeometry| image:: /static/common/check_geometry.png
   :width: 1.5em
.. |checkQgisVersion| image:: /static/common/mActionCheckQgisVersion.png
   :width: 1.5em
.. |checkbox| image:: /static/common/checkbox.png
   :width: 1.3em
.. |circularStringCurvePoint| image:: /static/common/mActionCircularStringCurvePoint.png
   :width: 1.5em
.. |circularStringRadius| image:: /static/common/mActionCircularStringRadius.png
   :width: 1.5em
.. |clip| image:: /static/common/clip.png
   :width: 1.5em
.. |collapseTree| image:: /static/common/mActionCollapseTree.png
   :width: 1.5em
.. |colorBox| image:: /static/common/mIconColorBox.png
   :width: 1.5em
.. |colorPicker| image:: /static/common/mIconColorPicker.png
   :width: 1.5em
.. |colorSwatches| image:: /static/common/mIconColorSwatches.png
   :width: 1.5em
.. |colorWheel| image:: /static/common/mIconColorWheel.png
   :width: 1.5em
.. |conditionalFormatting| image:: /static/common/mActionConditionalFormatting.png
   :width: 1.5em
.. |contextHelp| image:: /static/common/mActionContextHelp.png
   :width: 1.5em
.. |convexHull| image:: /static/common/convex_hull.png
   :width: 1.5em
.. |coordinateCapture| image:: /static/common/coordinate_capture.png
   :width: 1.5em
.. |copySelected| image:: /static/common/mActionCopySelected.png
   :width: 1.5em
.. |copyrightLabel| image:: /static/common/copyright_label.png
   :width: 1.5em
.. |createMemory| image:: /static/common/mActionCreateMemory.png
   :width: 1.5em
.. |crs| image:: /static/common/CRS.png
   :width: 1.5em
.. |customProjection| image:: /static/common/mActionCustomProjection.png
   :width: 1.5em
.. |dataDefineError| image:: /static/common/mIconDataDefineError.png
   :width: 1.5em
.. |dataDefineExpressionError| image:: /static/common/mIconDataDefineExpressionError.png
   :width: 1.5em
.. |dataDefineExpressionOn| image:: /static/common/mIconDataDefineExpressionOn.png
   :width: 1.5em
.. |dataDefineOn| image:: /static/common/mIconDataDefineOn.png
   :width: 1.5em
.. |dataDefined| image:: /static/common/mIconDataDefine.png
   :width: 1.5em
.. |dbManager| image:: /static/common/dbmanager.png
   :width: 1.5em
.. |defineProjection| image:: /static/common/define_projection.png
   :width: 1.5em
.. |degrees| unicode:: 0x00B0
   :ltrim:
.. |delaunay| image:: /static/common/delaunay.png
   :width: 1.5em
.. |deleteAttribute| image:: /static/common/mActionDeleteAttribute.png
   :width: 1.5em
.. |deletePart| image:: /static/common/mActionDeletePart.png
   :width: 2em
.. |deleteRing| image:: /static/common/mActionDeleteRing.png
   :width: 2em
.. |deleteSelected| image:: /static/common/mActionDeleteSelected.png
   :width: 1.5em
.. |delimitedText| image:: /static/common/delimited_text.png
   :width: 1.5em
.. |dependencies| image:: /static/common/dependencies.png
   :width: 1.5em
.. |deselectAll| image:: /static/common/mActionDeselectAll.png
   :width: 1.5em
.. |diagram| image:: /static/common/diagram.png
   :width: 2em
.. |diagramNone| image:: /static/common/diagramNone.png
   :width: 1.5em
.. |difference| image:: /static/common/difference.png
   :width: 1.5em
.. |dissolve| image:: /static/common/dissolve.png
   :width: 1.5em
.. |draw| image:: /static/common/mActionDraw.png
   :width: 1.5em
.. |duplicateLayout| image:: /static/common/mActionDuplicateComposer.png
   :width: 1.5em
.. |dxf2shpConverter| image:: /static/common/dxf2shp_converter.png
   :width: 1.5em
.. |editCopy| image:: /static/common/mActionEditCopy.png
   :width: 1.5em
.. |editCut| image:: /static/common/mActionEditCut.png
   :width: 1.5em
.. |editMetadata| image:: /static/common/editmetadata.png
   :width: 1.5em
.. |editNodesShape| image:: /static/common/mActionEditNodesShape.png
   :width: 1.5em
.. |editPaste| image:: /static/common/mActionEditPaste.png
   :width: 1.5em
.. |eventBrowser| image:: /static/common/event_browser.png
   :width: 1.5em
.. |eventId| image:: /static/common/event_id.png
   :width: 1.5em
.. |evisConnect| image:: /static/common/evis_connect.png
   :width: 1.5em
.. |evisFile| image:: /static/common/evis_file.png
   :width: 1.5em
.. |expandNewTree| image:: /static/common/mActionExpandNewTree.png
   :width: 1.5em
.. |expandTree| image:: /static/common/mActionExpandTree.png
   :width: 1.5em
.. |exportGeometry| image:: /static/common/export_geometry.png
   :width: 1.5em
.. |exportProjection| image:: /static/common/export_projection.png
   :width: 1.5em
.. |expression| image:: /static/common/mIconExpression.png
   :width: 1.5em
.. |expressionFilter| image:: /static/common/mIconExpressionFilter.png
   :width: 1.5em
.. |expressionSelect| image:: /static/common/mIconExpressionSelect.png
   :width: 1.5em
.. |extents| image:: /static/common/extents.png
   :width: 1.5em
.. |extractNodes| image:: /static/common/extract_nodes.png
   :width: 1.5em
.. |fileExit| image:: /static/common/mActionFileExit.png
.. |fileNew| image:: /static/common/mActionFileNew.png
   :width: 1.5em
.. |fileOpen| image:: /static/common/mActionFileOpen.png
   :width: 1.5em
.. |filePrint| image:: /static/common/mActionFilePrint.png
   :width: 1.5em
.. |fileSave| image:: /static/common/mActionFileSave.png
   :width: 1.5em
.. |fileSaveAs| image:: /static/common/mActionFileSaveAs.png
   :width: 1.5em
.. |fillRing| image:: /static/common/mActionFillRing.png
   :width: 1.5em
.. |filter| image:: /static/common/mActionFilter.png
   :width: 1.5em
.. |filterMap| image:: /static/common/mActionFilterMap.png
   :width: 1.5em
.. |folder| image:: /static/common/mActionFolder.png
   :width: 1.5em
.. |formAnnotation| image:: /static/common/mActionFormAnnotation.png
   :width: 1.5em
.. |formSelect| image:: /static/common/mIconFormSelect.png
   :width: 1.5em
.. |formView| image:: /static/common/mActionFormView.png
   :width: 1.5em
.. |fullCumulativeStretch| image:: /static/common/mActionFullCumulativeCutStretch.png
   :width: 1.5em
.. |fullHistogramStretch| image:: /static/common/mActionFullHistogramStretch.png
   :width: 1.5em
.. |gdal| image:: /static/common/gdal.png
   :width: 1.5em
.. |gdalScript| image:: /static/common/mActionGDALScript.png
   :width: 1.5em
.. |general| image:: /static/common/general.png
   :width: 2em
.. |geographic| image:: /static/common/geographic.png
.. |geometryChecker| image:: /static/common/geometrychecker.png
   :width: 1.5em
.. |geometrySnapper| image:: /static/common/geometrysnapper.png
   :width: 1.5em
.. |georeferencer| image:: /static/common/georeferencer.png
   :width: 1.5em
.. |gpsImporter| image:: /static/common/gps_importer.png
   :width: 1.5em
.. |gpsTrackBarChart| image:: /static/common/gpstrack_barchart.png
   :width: 1.5em
.. |gpsTrackPolarChart| image:: /static/common/gpstrack_polarchart.png
   :width: 1.5em
.. |graduatedSymbol| image:: /static/common/rendererGraduatedSymbol.png
   :width: 1.5em
.. |grass| image:: /static/common/grasslogo.png
   :width: 1.5em
.. |grassCloseMapset| image:: /static/common/grass_close_mapset.png
   :width: 1.5em
.. |grassNewMapset| image:: /static/common/grass_new_mapset.png
   :width: 1.5em
.. |grassOpenMapset| image:: /static/common/grass_open_mapset.png
   :width: 1.5em
.. |grassRegion| image:: /static/common/grass_region.png
   :width: 1.5em
.. |grassSetRegion| image:: /static/common/grass_set_region.png
   :width: 1.5em
.. |grassTools| image:: /static/common/grass_tools.png
   :width: 1.5em
.. |groupItems| image:: /static/common/mActionGroupItems.png
   :width: 1.5em
.. |heatmap| image:: /static/common/heatmap.png
   :width: 1.5em
.. |heatmapSymbol| image:: /static/common/rendererHeatmapSymbol.png
   :width: 1.5em
.. |helpAbout| image:: /static/common/mActionHelpAbout.png
   :width: 1.5em
.. |helpContents| image:: /static/common/mActionHelpContents.png
   :width: 1.5em
.. |helpSponsors| image:: /static/common/mActionHelpSponsors.png
   :width: 1.5em
.. |hideAllLayers| image:: /static/common/mActionHideAllLayers.png
   :width: 1.5em
.. |hideDeselectedLayers| image:: /static/common/mActionHideDeselectedLayers.png
   :width: 1.5em
.. |hideSelectedLayers| image:: /static/common/mActionHideSelectedLayers.png
   :width: 1.5em
.. |histogram| image:: /static/common/histogram.png
   :width: 1.5em
.. |history| image:: /static/common/mActionHistory.png
   :width: 1.5em
.. |htmlAnnotation| image:: /static/common/mActionHtmlAnnotation.png
   :width: 1.5em
.. |identify| image:: /static/common/mActionIdentify.png
   :width: 1.5em
.. |inOverview| image:: /static/common/mActionInOverview.png
   :width: 1.5em
.. |inputText| image:: /static/common/inputtext.png
.. |installPluginFromZip| image:: /static/common/mActionInstallPluginFromZip.png
   :width: 1.5em
.. |interpolation| image:: /static/common/interpolation.png
   :width: 1.5em
.. |intersect| image:: /static/common/intersect.png
   :width: 1.5em
.. |intersections| image:: /static/common/intersections.png
   :width: 1.5em
.. |invertSelection| image:: /static/common/mActionInvertSelection.png
   :width: 1.5em
.. |invertedSymbol| image:: /static/common/rendererInvertedSymbol.png
   :width: 1.5em
.. |join| image:: /static/common/join.png
   :width: 2em
.. |joinLocation| image:: /static/common/join_location.png
   :width: 1.5em
.. |kde| image:: /static/common/kde.png
   :width: 1.5em
.. |label| image:: /static/common/mActionLabel.png
   :width: 1.5em
.. |labeling| image:: /static/common/labelingSingle.png
   :width: 1.5em
.. |labelingNone| image:: /static/common/labelingNone.png
   :width: 1.5em
.. |labelingObstacle| image:: /static/common/labelingObstacle.png
   :width: 1.5em
.. |labelingRuleBased| image:: /static/common/labelingRuleBased.png
   :width: 1.5em
.. |layerExtent| image:: /static/common/layer_extent.png
   :width: 1.5em
.. |layoutManager| image:: /static/common/mActionComposerManager.png
   :width: 1.5em
.. |legend| image:: /static/common/legend.png
   :width: 1.5em
.. |linkGeorefToQGis| image:: /static/common/mActionLinkGeorefToQGis.png
   :width: 2.5em
.. |linkQGisToGeoref| image:: /static/common/mActionLinkQGisToGeoref.png
   :width: 2.5em
.. |locale| image:: /static/common/locale.png
   :width: 2em
.. |locked| image:: /static/common/locked.png
   :width: 1.5em
.. |lockedRepeat| image:: /static/common/lock_repeating.png
   :width: 1.5em
.. |lowerItems| image:: /static/common/mActionLowerItems.png
   :width: 1.5em
.. |mapIdentification| image:: /static/common/mActionMapIdentification.png
   :width: 1.5em
.. |mapTips| image:: /static/common/mActionMapTips.png
   :width: 1.5em
.. |matrix| image:: /static/common/matrix.png
   :width: 1.5em
.. |mean| image:: /static/common/mean.png
   :width: 1.5em
.. |measure| image:: /static/common/mActionMeasure.png
   :width: 1.5em
.. |measureAngle| image:: /static/common/mActionMeasureAngle.png
   :width: 1.5em
.. |measureArea| image:: /static/common/mActionMeasureArea.png
   :width: 1.5em
.. |mergeFeatAttributes| image:: /static/common/mActionMergeFeatureAttributes.png
   :width: 1.5em
.. |mergeFeatures| image:: /static/common/mActionMergeFeatures.png
   :width: 1.5em
.. |mergeShapes| image:: /static/common/merge_shapes.png
   :width: 1.5em
.. |metadata| image:: /static/common/metadata.png
   :width: 2em
.. |metasearch| image:: /static/common/MetaSearch.png
   :width: 1.5em
.. |moveFeature| image:: /static/common/mActionMoveFeature.png
   :width: 1.5em
.. |moveItemContent| image:: /static/common/mActionMoveItemContent.png
   :width: 1.5em
.. |moveItemsToBottom| image:: /static/common/mActionMoveItemsToBottom.png
   :width: 1.5em
.. |moveItemsToTop| image:: /static/common/mActionMoveItemsToTop.png
   :width: 1.5em
.. |multiEdit| image:: /static/common/mActionMultiEdit.png
   :width: 1.5em
.. |multiToSingle| image:: /static/common/multi_to_single.png
   :width: 1.5em
.. |neighbor| image:: /static/common/neighbour.png
   :width: 1.5em
.. |newAttribute| image:: /static/common/mActionNewAttribute.png
   :width: 1.5em
.. |newBookmark| image:: /static/common/mActionNewBookmark.png
   :width: 1.5em
.. |newGeoPackageLayer| image:: /static/common/mActionNewGeoPackageLayer.png
   :width: 1.5em
.. |newLayout| image:: /static/common/mActionNewComposer.png
   :width: 1.5em
.. |newMap| image:: /static/common/mActionNewMap.png
   :width: 1.5em
.. |newSpatiaLiteLayer| image:: /static/common/mActionNewSpatiaLiteLayer.png
   :width: 1.5em
.. |newTableRow| image:: /static/common/mActionNewTableRow.png
   :width: 1.5em
.. |newVectorLayer| image:: /static/common/mActionNewVectorLayer.png
   :width: 1.5em
.. |nix| image:: /static/common/nix.png
   :width: 1em
.. |nodeTool| image:: /static/common/mActionNodeTool.png
   :width: 1.5em
.. |northArrow| image:: /static/common/north_arrow.png
   :width: 1.5em
.. |nullSymbol| image:: /static/common/rendererNullSymbol.png
   :width: 1.5em
.. |offlineEditingCopy| image:: /static/common/offline_editing_copy.png
   :width: 1.5em
.. |offlineEditingSync| image:: /static/common/offline_editing_sync.png
   :width: 1.5em
.. |offsetCurve| image:: /static/common/mActionOffsetCurve.png
   :width: 1.5em
.. |offsetPointSymbols| image:: /static/common/mActionOffsetPointSymbols.png
   :width: 1.5em
.. |openTable| image:: /static/common/mActionOpenTable.png
   :width: 1.5em
.. |options| image:: /static/common/mActionOptions.png
   :width: 1em
.. |oracleRaster| image:: /static/common/oracleraster.png
   :width: 1.5em
.. |osmAddRelation| image:: /static/common/osm_addRelation.png
   :width: 1.5em
.. |osmCreateLine| image:: /static/common/osm_createLine.png
   :width: 1.5em
.. |osmCreatePoint| image:: /static/common/osm_createPoint.png
   :width: 1.5em
.. |osmCreatePolygon| image:: /static/common/osm_createPolygon.png
   :width: 1.5em
.. |osmCreateRelation| image:: /static/common/osm_createRelation.png
   :width: 1.5em
.. |osmDownload| image:: /static/common/osm_download.png
   :width: 1.5em
.. |osmEditRelation| image:: /static/common/osm_editRelation.png
   :width: 1.5em
.. |osmFeatureManager| image:: /static/common/osm_featureManager.png
   :width: 1.5em
.. |osmGenerateTags| image:: /static/common/osm_generateTags.png
   :width: 1.5em
.. |osmIdentify| image:: /static/common/osm_identify.png
   :width: 1.5em
.. |osmImport| image:: /static/common/osm_import.png
   :width: 1.5em
.. |osmLoad| image:: /static/common/osm_load.png
   :width: 1.5em
.. |osmMove| image:: /static/common/osm_move.png
   :width: 1.5em
.. |osmQuestionMark| image:: /static/common/osm_questionMark.png
   :width: 1.5em
.. |osmRemoveFeat| image:: /static/common/osm_removeFeat.png
   :width: 1.5em
.. |osmSave| image:: /static/common/osm_save.png
   :width: 1.5em
.. |osx| image:: /static/common/osx.png
   :width: 1em
.. |overlay| image:: /static/common/overlay.png
   :width: 1.5em
.. |paintEffects| image:: /static/common/mIconPaintEffects.png
   :width: 1.5em
.. |pan| image:: /static/common/mActionPan.png
   :width: 1.5em
.. |panToSelected| image:: /static/common/mActionPanToSelected.png
   :width: 1.5em
.. |pencil| image:: /static/common/pencil.png
   :width: 1.5em
.. |piechart| image:: /static/common/pie-chart.png
   :width: 1.5em
.. |plugin| image:: /static/common/plugin.png
   :width: 1.5em
.. |pluginInstaller| image:: /static/common/plugin_installer.png
   :width: 1.5em
.. |pointClusterSymbol| image:: /static/common/rendererPointClusterSymbol.png
   :width: 1.5em
.. |pointDisplacementSymbol| image:: /static/common/rendererPointDisplacementSymbol.png
   :width: 1.5em
.. |projectProperties| image:: /static/common/mActionProjectProperties.png
   :width: 1.5em
.. |projectionDisabled| image:: /static/common/mIconProjectionDisabled.png
   :width: 1.5em
.. |projectionEnabled| image:: /static/common/mIconProjectionEnabled.png
   :width: 1.5em
.. |propertiesWidget| image:: /static/common/mActionPropertiesWidget.png
   :width: 1.5em
.. |propertyItem| image:: /static/common/mActionPropertyItem.png
   :width: 1.5em
.. |qgisHomePage| image:: /static/common/mActionQgisHomePage.png
   :width: 1.5em
.. |radioButtonOff| image:: /static/common/radiobuttonoff.png
.. |radioButtonOn| image:: /static/common/radiobuttonon.png
.. |raiseItems| image:: /static/common/mActionRaiseItems.png
   :width: 1.5em
.. |randomPoints| image:: /static/common/random_points.png
   :width: 1.5em
.. |randomSelection| image:: /static/common/random_selection.png
   :width: 1.5em
.. |rasterInfo| image:: /static/common/raster-info.png
   :width: 1.5em
.. |rasterInterpolate| image:: /static/common/raster-interpolate.png
   :width: 1.5em
.. |rasterStats| image:: /static/common/raster-stats.png
   :width: 1.5em
.. |rasterTerrain| image:: /static/common/raster_terrain.png
   :width: 1.5em
.. |redo| image:: /static/common/mActionRedo.png
   :width: 1.5em
.. |regularPoints| image:: /static/common/regular_points.png
   :width: 1.5em
.. |removeAllOVerview| image:: /static/common/mActionRemoveAllFromOverview.png
   :width: 1.5em
.. |removeLayer| image:: /static/common/mActionRemoveLayer.png
   :width: 1.5em
.. |rendering| image:: /static/common/rendering.png
   :width: 1.5em
.. |reshape| image:: /static/common/mActionReshape.png
   :width: 1.5em
.. |rotateFeature| image:: /static/common/mActionRotateFeature.png
   :width: 1.5em
.. |rotatePointSymbols| image:: /static/common/mActionRotatePointSymbols.png
   :width: 1.5em
.. |ruleBasedSymbol| image:: /static/common/rendererRuleBasedSymbol.png
   :width: 1.5em
.. |saveAsPDF| image:: /static/common/mActionSaveAsPDF.png
   :width: 1.5em
.. |saveAsSVG| image:: /static/common/mActionSaveAsSVG.png
   :width: 1.5em
.. |saveEdits| image:: /static/common/mActionSaveEdits.png
   :width: 1.5em
.. |saveMapAsImage| image:: /static/common/mActionSaveMapAsImage.png
   :width: 1.5em
.. |scaleBar| image:: /static/common/mActionScaleBar.png
   :width: 1.5em
.. |select| image:: /static/common/mActionSelect.png
   :width: 1.5em
.. |selectAll| image:: /static/common/mActionSelectAll.png
   :width: 1.5em
.. |selectAllTree| image:: /static/common/mActionSelectAllTree.png
   :width: 1.5em
.. |selectColor| image:: /static/common/selectcolor.png
.. |selectFreehand| image:: /static/common/mActionSelectFreehand.png
   :width: 1.5em
.. |selectLocation| image:: /static/common/select_location.png
   :width: 1.5em
.. |selectNumber| image:: /static/common/selectnumber.png
   :width: 2.8em
.. |selectPolygon| image:: /static/common/mActionSelectPolygon.png
   :width: 1.5em
.. |selectRadius| image:: /static/common/mActionSelectRadius.png
   :width: 1.5em
.. |selectRectangle| image:: /static/common/mActionSelectRectangle.png
   :width: 1.5em
.. |selectString| image:: /static/common/selectstring.png
   :width: 2.5em
.. |selectedToTop| image:: /static/common/mActionSelectedToTop.png
   :width: 1.5em
.. |setProjection| image:: /static/common/mActionSetProjection.png
   :width: 1.5em
.. |settings| image:: /static/common/settings.png
   :width: 1.5em
.. |showAllLayers| image:: /static/common/mActionShowAllLayers.png
   :width: 1.5em
.. |showBookmarks| image:: /static/common/mActionShowBookmarks.png
   :width: 1.5em
.. |showMapTheme| image:: /static/common/mActionShowPresets.png
   :width: 1.5em
.. |showPluginManager| image:: /static/common/mActionShowPluginManager.png
   :width: 1.5em
.. |showRasterCalculator| image:: /static/common/mActionShowRasterCalculator.png
   :width: 1.5em
.. |showSelectedLayers| image:: /static/common/mActionShowSelectedLayers.png
   :width: 1.5em
.. |signMinus| image:: /static/common/symbologyRemove.png
   :width: 1.5em
.. |signPlus| image:: /static/common/symbologyAdd.png
   :width: 1.5em
.. |simplify| image:: /static/common/simplify.png
   :width: 1.5em
.. |simplifyFeatures| image:: /static/common/mActionSimplify.png
   :width: 2em
.. |singleSymbol| image:: /static/common/rendererSingleSymbol.png
   :width: 1.5em
.. |singleToMulti| image:: /static/common/single_to_multi.png
   :width: 1.5em
.. |slider| image:: /static/common/slider.png
.. |snapping| image:: /static/common/mIconSnapping.png
   :width: 1.5em
.. |sort| image:: /static/common/sort.png
   :width: 1.5em
.. |sourceFields| image:: /static/common/mSourceFields.png
   :width: 1.5em
.. |splitFeatures| image:: /static/common/mActionSplitFeatures.png
   :width: 1.5em
.. |splitLayer| image:: /static/common/split_layer.png
   :width: 1.5em
.. |splitParts| image:: /static/common/mActionSplitParts.png
   :width: 1.5em
.. |startGeoref| image:: /static/common/mActionStartGeoref.png
   :width: 1.5em
.. |stylePreset| image:: /static/common/stylepreset.png
   :width: 1.5em
.. |subSelection| image:: /static/common/sub_selection.png
   :width: 1.5em
.. |sum| image:: /static/common/mActionSum.png
   :width: 1.5em
.. |sumLines| image:: /static/common/sum_lines.png
   :width: 1.5em
.. |sumPoints| image:: /static/common/sum_points.png
   :width: 1.5em
.. |svgAnnotation| image:: /static/common/mActionSvgAnnotation.png
   :width: 1.5em
.. |symDifference| image:: /static/common/sym_difference.png
   :width: 1.5em
.. |symbology| image:: /static/common/symbology.png
   :width: 2em
.. |system| image:: /static/common/system.png
   :width: 1.5em
.. |tab| image:: /static/common/tab.png
   :width: 1.5em
.. |text| image:: /static/common/text.png
   :width: 1.5em
.. |textAnnotation| image:: /static/common/mActionTextAnnotation.png
   :width: 1.5em
.. |toLines| image:: /static/common/to_lines.png
   :width: 1.5em
.. |toggleEditing| image:: /static/common/mActionToggleEditing.png
   :width: 1.5em
.. |topologyChecker| image:: /static/common/topol.png
   :width: 1.5em
.. |touch| image:: /static/common/mActionTouch.png
   :width: 1.5em
.. |tracing| image:: /static/common/mActionTracing.png
   :width: 1.5em
.. |tracking| image:: /static/common/tracking.png
   :width: 1.5em
.. |unchecked| image:: /static/common/checkbox_unchecked.png
   :width: 1.3em
.. |undo| image:: /static/common/mActionUndo.png
   :width: 1.5em
.. |union| image:: /static/common/union.png
   :width: 1.5em
.. |unique| image:: /static/common/unique.png
   :width: 1.5em
.. |unlocked| image:: /static/common/unlocked.png
   :width: 1.5em
.. |vectorGrid| image:: /static/common/vector_grid.png
   :width: 1.5em
.. |virtualLayer| image:: /static/common/mActionAddVirtualLayer.png
   :width: 1.5em
.. |wcs| image:: /static/common/mActionAddWcsLayer.png
   :width: 1.5em
.. |wfs| image:: /static/common/mActionAddWfsLayer.png
   :width: 1.5em
.. |win| image:: /static/common/win.png
   :width: 1em
.. |wms| image:: /static/common/mActionAddWmsLayer.png
   :width: 1.5em
.. |zip| image:: /static/common/mIconZip.png
   :width: 2em
.. |zoomActual| image:: /static/common/mActionZoomActual.png
   :width: 1.5em
.. |zoomFullExtent| image:: /static/common/mActionZoomFullExtent.png
   :width: 1.5em
.. |zoomIn| image:: /static/common/mActionZoomIn.png
   :width: 1.5em
.. |zoomLast| image:: /static/common/mActionZoomLast.png
   :width: 1.5em
.. |zoomNext| image:: /static/common/mActionZoomNext.png
   :width: 1.5em
.. |zoomOut| image:: /static/common/mActionZoomOut.png
   :width: 1.5em
.. |zoomToLayer| image:: /static/common/mActionZoomToLayer.png
   :width: 1.5em
.. |zoomToSelected| image:: /static/common/mActionZoomToSelected.png
   :width: 1.5em