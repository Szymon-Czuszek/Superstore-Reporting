# Superstore-Reporting
This project aims to show capabilities of Alteryx software on the Kaggle data named "Superstore". The project includes creation of an analytic application, spatial analysis, creating report visualisations, exploratory data analysis, and a unique Alteryx approach to the traveling salesman problem.

### Workflow graphical representation: Loading Data.
- Using Alteryx Tools: Input Data Tool, Auto Field Tool, DateTime Tool, Join Tool, Union Tool, Formula Tool, Select Tool, Create Points Tool, File Browse Tool, Text Box Tool, Action Tool, Radio Button Tool, Summarize Tool.
**![WF1.png](Workflow-Screens/WF1.png)**

### Workflow graphical representation: Data manipulation.
- Using Alteryx Tools: Summarize Tool, Formula Tool, Sample Tool, Sort Tool, Join Tool, Union Tool, Filter Tool, and more.
**![WF2.png](Workflow-Screens/WF2.png)**

### Workflow graphical representation: Aggregation and reporting.
- Using Alteryx Tools: Union Tool, Interactive Chart Tool, Layout Tool, and more
**![WF3.png](Workflow-Screens/WF3.png)**

### Workflow graphical representation: Aggregation and reporting.
- Using Alteryx Tools: Union Tool, Interactive Chart Tool, Layout Tool, and more
**![WF4.png](Workflow-Screens/WF4.png)**

### Workflow graphical representation: Data Investigation.
- Using Alteryx Tools: Spearman Correlation, Pearson Correlation, and more.
**![WF5.png](Workflow-Screens/WF5.png)**

### Workflow graphical representation: Spatial Analysis.
- Using Alteryx Tools: Poly-Build Tool, Make Points Tool.
**![WF6.png](Workflow-Screens/WF6.png)**

## Iterative Macro used in the "Superstore" project.
This [iterative macro](Shortest%20Route.yxmc) uses iterative process to find the nearest location using spatial analytics. This macro aims to solve the "Traveling Salesman Problem", but it needs an upstream macro that will run this process for other combination of starting points, which is further solved in "Shortest Route Batch" Macro.

### Alteryx Custom Made Macro Group
- Using Custom Made Iterative Macro
**![CustomMacro3.png](Workflow-Screens/CustomMacro3.png)**

### Alteryx Custom Made Macro Group
- Investigating Custom Made Iterative Macro
**![IterativeMacro.png](Workflow-Screens/IterativeMacro.png)**

## Batch Macro used in the "Superstore" Project.
This [batch macro](Shortest%20Route%20Batch.yxmc) uses batch process to find the nearest location using spatial analytics. This macro aims to solve the "Traveling Salesman Problem", and it is used to produce many outputs using batches. It needs an upstream macro, that will actually find the most optimal route, using MIN function, which is tackled further in the "Shortest Route Checker" Standard Macro.

### Alteryx Custom Made Macro Group
- Using Custom Made Batch Macro
**![CustomMacro2.png](Workflow-Screens/CustomMacro2.png)**

### Alteryx Custom Made Macro Group
- Investigating Custom Made Batch Macro
**![BatchMacro.png](Workflow-Screens/BatchMacro.png)**

## Standard Macro used in "Superstore" project.
This [standard macro](Shortest%20Route%20Checker.yxmc) feeds iterative and batch process to find the nearest location using spatial analytics. This macro aims to solve the "Traveling Salesman Problem", but it's limitation is the longer run times, depending on the amount of locations it needs to connect and check.

### Alteryx Custom Made Macro Group
- Using Custom Made Standard Macro
**![CustomMacro.png](Workflow-Screens/CustomMacro.png)**

### Alteryx Custom Made Macro Group
- Investigating Custom Made Standard Macro
**![Custom-Made Standard Macro](Workflow-Screens/StandardMacro.png)**

## Project "Superstore" - Analytic Application only.
An [analytic app](ProjectSuperstore.yxwz) containing the user interface, spatial, reporting, macros, and other advanced functionalities.

## Workflow-Screens Folder
The folder contains screens of the workflow, as is in the file.

### <img src="https://community.alteryx.com/t5/image/serverpage/image-id/9469i39AD90998C11FF7D/image-size/original?v=v2&px=-1" width="60" /> [Tool Mastery](https://community.alteryx.com/t5/Tool-Mastery/Tool-Mastery-Action/ta-p/35500) | Alteryx Interface Tool Group | Action Tool

#### Alteryx Interface Tool Group
- Using Action Tool in Alteryx
**![Action.png](Workflow-Screens/Action.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-a859e43c-5d1c-398e-ebaf-5114987a3544.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/join/append-fields-tool.html) | Alteryx Join Tool Group | Append Fields Tool

#### Alteryx Join Tool Group
- Using Append Fields Tool in Alteryx
**![Append.png](Workflow-Screens/Append.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-b7347050-71b7-b0da-cd14-6420f0a8eca9.png" width="60" /> [Tool Mastery](https://community.alteryx.com/t5/Tool-Mastery/Tool-Mastery-Auto-Field/ta-p/49731?lightbox-message-images-49731=13686i8C7DFB7FE4CCD355) | Alteryx Preparation Tool Group | Auto Field Tool

#### Using Auto Field Tool in Alteryx - Input
- Screen-shot below presents the configuration of the auto filed tool. The metadata tab is selected on purpouse, as the tool will convert the string data types, as in the output anchor. The configuration of the tool comes down only to selection of the fileds, of which types we whish to adjust.
**![Auto1.png](Workflow-Screens/Auto1.png)** 

#### Using Auto Field Tool in Alteryx - Output
- Screen-shot below presents the output anchor of the auto field tool, with already converted file types. As seen, some types like double or byte were easily recognizable by the tool, and got changed from string.
**![Auto2.png](Workflow-Screens/Auto2.png)**

### <img src="https://community.alteryx.com/t5/image/serverpage/image-id/8175i912ACB670A1F9F1C/image-size/original?v=v2&px=-1" width="60" /> [Tool Mastery](https://community.alteryx.com/t5/Tool-Mastery/Tool-Mastery-Basic-Data-Profile/ta-p/28610) | Alteryx Data Investigation Tool Group | Basic Data Profile Tool

#### Alteryx Data Investigation Group
- Using Basic Data Profile Tool in Alteryx
**![BasicDataProfile.png](Workflow-Screens/BasicDataProfile.png)**

### <img src="https://community.alteryx.com/t5/image/serverpage/image-id/9900iAB3EC61959EFE81D/image-size/large?v=v2&px=999" width="60" /> [Tool Mastery](https://community.alteryx.com/t5/Tool-Mastery/Tool-Mastery-Browse/ta-p/1208) | Alteryx In/Out Tool Group | Browse Tool

#### Alteryx In/Out Group
- Using Browse Tool in Alteryx
**![Browse.png](Workflow-Screens/Browse.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-da6558a8-7881-c24f-4dbd-23ab3ba4ada1.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/spatial/poly-build-tool.html#poly-build-tool) | Alteryx Spatial Tool Group | Poly-Build Tool

#### Alteryx Spatial Group
- Using Poly-Build Tool in Alteryx
**![BuildingSequenceLine.png](Workflow-Screens/BuildingSequenceLine.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-e3bb418c-d6cc-4b4b-136c-8d60034b6242.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/reporting/interactive-chart-tool.html) | Alteryx Reporting Tool Group | Interactive Chart Tool

#### Alteryx Reporting Group
- Using Interactive Chart Tool in Alteryx
**![Chart.png](Workflow-Screens/Chart.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-56a84855-008e-d04c-d237-a04c11ddd488.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/transform/count-records-tool.html##) | Alteryx Interface Tool Group | Control Parameter Tool

#### Alteryx Interface Group
- Using Control Parameter Tool in Alteryx
**![ControlParameter.png](Workflow-Screens/ControlParameter.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-9b8a711a-c9ee-ef6b-7e54-6f2f4a40d1db.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/transform/count-records-tool.html##) | Alteryx Transform Tool Group | Count Records Tool

#### Alteryx Transformation Group
- Using Count Records Tool in Alteryx
**![Count.png](Workflow-Screens/Count.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-b9c2ec12-3d7e-1bc1-541b-08e82f62ad23.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/parse/datetime-tool.html) | Alteryx Parse Tool Group | DateTime Tool

#### Alteryx Parse Group
- Using DateTime Tool in Alteryx
**![DateParse.png](Workflow-Screens/DateParse.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-8b46f1d2-43ef-5744-5b66-936ff167f23d.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/data-investigation/field-summary-tool.html) | Alteryx Data Investigation Tool Group | Field Summary Tool

#### Alteryx Data Investigation Group
- Using Field Summary Tool in Alteryx
**![FieldSummary.png](Workflow-Screens/FieldSummary.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-69122228-92d1-770a-c737-0ffe904b58ad.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/preparation/filter-tool.html) | Alteryx Preparation Tool Group | Filter Tool

#### Alteryx Preparation Group
- Using Filter Tool in Alteryx
**![Filter.png](Workflow-Screens/Filter.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-4da60bda-dd8b-31d5-aa21-adfa8a201b08.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/reporting/report-footer-tool.html) | Alteryx Reporting Tool Group | Report Footer Tool

#### Alteryx Reporting Group
- Using Report Footer Tool in Alteryx
**![Foot.png](Workflow-Screens/Foot.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-9dc01e86-c9f6-f365-2a11-4528d15c7499.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/preparation/formula-tool.html) | Alteryx Preparation Tool Group | Formula Tool

#### Alteryx Preparation Group
- Using Formula Tool in Alteryx
**![Formula.png](Workflow-Screens/Formula.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-c83f681c-0283-6b3a-504e-b331ebd7cc3f.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/reporting/report-header-tool.html) | Alteryx Reporting Tool Group | Report Header Tool

#### Alteryx Reporting Group
- Using Report Header Tool in Alteryx
**![Head.png](Workflow-Screens/Head.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-f9b13cd1-5718-a091-fdfa-c936c74743db.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/join/join-tool.html) | Alteryx Join Tool Group | Join Tool

#### Alteryx Join Tool Group
- Using Join Tool in Alteryx
**![Join.png](Workflow-Screens/Join.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-8ecd5bdf-cd31-a5fb-f6fd-7b90443cee38.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/reporting/layout-tool.html) | Alteryx Reporting Tool Group | Layout Tool

#### Alteryx Reporting Group
- Using Report Header Tool in Alteryx
**![Layout.png](Workflow-Screens/Layout.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-d4fa5b87-25bb-b657-ae17-8bfa92c3f4d4.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/developer/message-tool.html) | Alteryx Developer Tool Group | Message Tool

#### Alteryx Developer Tool Group
- Using Message Tool in Alteryx
**![Msg.png](Workflow-Screens/Msg.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-a1e53169-3eea-ba91-aa40-b58af5ec610b.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/interface-tools/numeric-up-down-tool.html) | Alteryx Interface Tool Group | Numeric Up Down Tool

#### Alteryx Interface Tool Group
- Using Numeric Up Down Tool in Alteryx
**![NumericUpDown.png](Workflow-Screens/NumericUpDown.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-17670fc7-0e8c-699e-1907-cf66553471eb.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/data-investigation/pearson-correlation-tool.html) | Alteryx Data Investigation Tool Group | Pearson Correlation Tool

#### Alteryx Data Investigation Group
- Using Pearson Correlation Tool in Alteryx
**![Pearson.png](Workflow-Screens/Pearson.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-b4b16910-3ed6-7de0-76d7-de55a231c245.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/preparation/random---sample-tool.html) | Alteryx Preparation Tool Group | Random % Sample Tool

#### Alteryx Data Preparation Group
- Using Random Sample Tool in Alteryx
**![Random.png](Workflow-Screens/Random.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-915aa92e-03af-6633-3a22-cdf42b45f1a0.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/preparation/record-id-tool.html) | Alteryx Preparation Tool Group | Record ID Tool

#### Alteryx Data Preparation Group
- Using Record ID Tool in Alteryx
**![Record ID.png](Workflow-Screens/Record%20ID.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-c0b1d777-4b86-3f21-687f-75255991ba5d.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/reporting/render-tool.html) | Alteryx Reporting Tool Group | Render Tool

#### Alteryx Reporting Group
- Using Render Tool in Alteryx
**![Render.png](Workflow-Screens/Render.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-935e0072-f113-fb2d-d615-0348c7a755c1.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/reporting/report-map-tool.html) | Alteryx Reporting Tool Group | Report Map Tool

#### Alteryx Reporting Group
- Using Report Map Tool in Alteryx
**![ReportMap.png](Workflow-Screens/ReportMap.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-9ff5db68-a24a-c353-89d2-7fe601852fe3.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/reporting/report-text-tool.html) | Alteryx Reporting Tool Group | Report Text Tool

#### Alteryx Reporting Group
- Using Report Text Tool in Alteryx
**![ReportText.png](Workflow-Screens/ReportText.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-8fec8c20-cc8b-21e1-195f-c698c45344fd.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/transform/running-total-tool.html) | Alteryx Transform Tool Group | Running Total Tool

#### Alteryx Transformation Group
- Using Running Total Tool in Alteryx
**![RunningTotal.png](Workflow-Screens/RunningTotal.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-d779826a-75e6-81f3-2e95-4c92c87cad7b.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/preparation/select-tool.html) | Alteryx Preparation Tool Group | Select Tool

#### Alteryx Data Preparation Group
- Using Select Tool in Alteryx
**![Select.png](Workflow-Screens/Select.png)**

### <img src="https://help.alteryx.com/current/en/image/uuid-3c3c14a7-a68a-dad6-83ec-a92ac54473a1.png" width="60" /> [Tool Mastery](https://help.alteryx.com/current/en/designer/tools/developer/dynamic-select-tool.html) | Alteryx Developer Tool Group | Dynamic Select Tool

#### Alteryx Developer Tool Group
- Using Dynamic Select Tool in Alteryx
**![SelectDynamic.png](Workflow-Screens/SelectDynamic.png)**

#### Alteryx Data Preparation Group
- Using Sort Tool in Alteryx
**![Sort.png](Workflow-Screens/Sort.png)**

#### Alteryx Data Investigation Group
- Using Spearman Correlation Tool in Alteryx
**![Spearman Tool](Workflow-Screens/Spearman.png)**

#### Alteryx Transformation Group
- Using Summarize Tool in Alteryx
**![Summarize Tool](Workflow-Screens/Summarize.png)**

#### Alteryx Reporting Group
- Using Table Tool in Alteryx
**![Table.png](Workflow-Screens/Table.png)**

#### Alteryx Join Tool Group
- Using Union Tool in Alteryx
**![UnionTool.png](Workflow-Screens/UnionTool.png)**

## Disclaimer
The images used in this README are the property of Alteryx, Inc. and are used here for informational purposes only. All rights to these images are retained by Alteryx, Inc. No copyright infringement is intended.
