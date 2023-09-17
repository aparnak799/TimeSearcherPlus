# TimeSearcherPlus - Technical Documentation
TimeSearcher+ is an interactive temporal data querying widget. Designed for standalone or integrated use in larger applications, its hallmark is direct manipulation of temporal datasets with multiple attributes. The widget introduces a reactive feature, a significant enhancement from its predecessors, which meets the demands of domain experts and users alike. Users can craft bounding boxes, termed "TimeBoxes," which act as constraints on the dataset, enabling them to meticulously select data intervals. Subsequently, they can analyze and compare trends within these intervals, grouping their findings for later reference or hiding.

## Table of Contents
- src
  - TimeSearcher.js
  - Timeline.js
  - TimelineOverview.js
  - TimeLineDetails.js
  - BVH.js 
  - BrushInteraction.js 
  - BrushTooltipEditable.js
  - utils.js
  - index.js
- examples
  - canguro.html, index.html
  - curvasPC.json, curvasPeso.json, curvasTalla.json
  - sp500_20-22.csv, tData10000.csv, tDataAll.csv, tDataG.csv
- Additional files
  - CODE_OF_CONDUCT.md
  - rollup.config.mjs
## src - Modules
### TimeSearcher.js
#### Purpose:
Central widget function with brush and group attributes. Initialization and onChange functions of different components of the TimeSearcher+ widget.
#### Functions and Classes:
1. initBrushesControls()
2. computeBrushColor(groupId)
3. onAddBrushGroup()
4. onChangeNonSelected(newState)
5. onChangeBrushGroupState(id, newState)
6. onRemoveBrushGroup(id)
7. onSelectBrushGroup(id)
8. onChangeSelectedBrush(brush)
9. renderBrushesControls()
10. initDomains({ xDataType, groupedData, fData })
11. init()
12. updateBrushSpinBox(selection)
13. emptyBrushSpinBox()
14. generateBrushCoordinatesDiv()
15. generateDataSelectionDiv()
16. filterDatabyDataGroups(dataSelected, dataNotSelected)
17. onGroupDataChange()
18. initDetails({ xDataType, fData })
19. onSpinboxChange(sourceEvent)
20. getSpinBoxValues()
21. onArrowRigth()
22. onArrowLeft()
23. onArrowDown()
24. onArrowUp()
25. render(dataSelected, dataNotSelected, hasSelection)
26. getBrushGroupsMedians(data)
27. onSelectionChange(
    newDataSelected = dataSelected,
    newDataNotSelected = dataNotSelected,
    hasSelection = brushes.hasSelection(),
    update = true
  )
28. recreateBrushes(value)
29. onBrushGroupsChange()
30. triggerValueUpdate(sel = divOverview.value)
31. sentSelection(selection, update)
32. sentEvent(customEvent)
33. onTimeSearcherEvent(event)
34. onUpdateEvent(tsId)
35. changeBrushNames()
36. filterByExternalSelected(dataSelected, dataNotSelected)


#### Dependencies:

### Timeline.js
#### Purpose:
Renders a SVG or HTML Canvas element representation of a timeline. Includes customization for various parameters such as width, height, scale etc.
#### Functions and Classes:
#### Dependencies:

### TimeLineOverview.js
#### Purpose:
Renders an overview of the timeline with provisions for selecting and highlighting certain subsets of data.
#### Functions and Classes:
#### Dependencies:
### TimelineDetails.js
#### Purpose:
Renders an enhanced and detailed view of specific components of the timeline in an optimized manner.
#### Functions and Classes:
#### Dependencies:
### BVH.js
#### Purpose:
Bounding Volume Hierarchy structure (BVH) to query which data lines intersect a given region in the timeline.
#### Functions and Classes:
#### Dependencies:
### BrushInteaction.js
#### Purpose:
Defines the interactive behaviors of the brush feature of the widget. These include: movement, selection, grouping etc.
#### Functions and Classes:
#### Dependencies:
### BrushTooltipEditable.js
#### Purpose:
#### Functions and Classes:
#### Dependencies:
### utils.js
#### Purpose:
#### Functions and Classes:
#### Dependencies:
### index.js
#### Purpose:
#### Functions and Classes:
#### Dependencies:


## examples - Modules
### canguro.html
#### Purpose:
#### Functions and Classes:
#### Dependencies:
### index.html
#### Purpose:
#### Functions and Classes:
#### Dependencies:

