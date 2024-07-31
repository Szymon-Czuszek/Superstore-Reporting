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

#### Alteryx Interface Tool Group
- Using Action Tool in Alteryx
**![Action.png](Workflow-Screens/Action.png)**

#### Alteryx Join Tool Group
- Using Append Fields Tool in Alteryx
**![Append.png](Workflow-Screens/Append.png)**

### ![pic](https://community.alteryx.com/t5/image/serverpage/image-id/13686i8C7DFB7FE4CCD355?v=v2) [Tool Mastery](https://community.alteryx.com/t5/Tool-Mastery/Tool-Mastery-Auto-Field/ta-p/49731?lightbox-message-images-49731=13686i8C7DFB7FE4CCD355) | Alteryx Preparation Tool Group | Auto Field Tool

#### Using Auto Field Tool in Alteryx - Input
- Screen-shot below presents the configuration of the auto filed tool. The metadata tab is selected on purpouse, as the tool will convert the string data types, as in the output anchor. The configuration of the tool comes down only to selection of the fileds, of which types we whish to adjust.
**![Auto1.png](Workflow-Screens/Auto1.png)** 

#### Using Auto Field Tool in Alteryx - Output
- Screen-shot below presents the output anchor of the auto field tool, with already converted file types. As seen, some types like double or byte were easily recognizable by the tool, and got changed from string.
**![Auto2.png](Workflow-Screens/Auto2.png)**

#### Alteryx Data Investigation Group
- Using Basic Data Profile Tool in Alteryx
**![BasicDataProfile.png](Workflow-Screens/BasicDataProfile.png)**

#### Alteryx In/Out Group
- Using Browse Tool in Alteryx
**![Browse.png](Workflow-Screens/Browse.png)**

#### Alteryx Spatial Group
- Using Poly-Build Tool in Alteryx
**![BuildingSequenceLine.png](Workflow-Screens/BuildingSequenceLine.png)**

#### Alteryx Reporting Group
- Using Interactive Chart Tool in Alteryx
**![Chart.png](Workflow-Screens/Chart.png)**

#### Alteryx Interface Group
- Using Control Parameter Tool in Alteryx
**![ControlParameter.png](Workflow-Screens/ControlParameter.png)**

#### Alteryx Transformation Group
- Using Count Records Tool in Alteryx
**![Count.png](Workflow-Screens/Count.png)**

#### Alteryx Parse Group
- Using Date Parse Tool in Alteryx
**![DateParse.png](Workflow-Screens/DateParse.png)**

#### Alteryx Data Investigation Group
- Using Field Summary Tool in Alteryx
**![FieldSummary.png](Workflow-Screens/FieldSummary.png)**

#### Alteryx Preparation Group
- Using Filter Tool in Alteryx
**![Filter.png](Workflow-Screens/Filter.png)**

#### Alteryx Reporting Group
- Using Report Footer Tool in Alteryx
**![Foot.png](Workflow-Screens/Foot.png)**

#### Alteryx Preparation Group
- Using Formula Tool in Alteryx
**![Formula.png](Workflow-Screens/Formula.png)**

#### Alteryx Reporting Group
- Using Report Header Tool in Alteryx
**![Head.png](Workflow-Screens/Head.png)**

#### Alteryx Join Tool Group
- Using Join Tool in Alteryx
**![Join.png](Workflow-Screens/Join.png)**

#### Alteryx Reporting Group
- Using Report Header Tool in Alteryx
**![Layout.png](Workflow-Screens/Layout.png)**

#### Alteryx Developer Tool Group
- Using Message Tool in Alteryx
**![Msg.png](Workflow-Screens/Msg.png)**

#### Alteryx Interface Tool Group
- Using Numeric Up Down Tool in Alteryx
**![NumericUpDown.png](Workflow-Screens/NumericUpDown.png)**

#### Alteryx Data Investigation Group
- Using Pearson Correlation Tool in Alteryx
**![Pearson.png](Workflow-Screens/Pearson.png)**

#### Alteryx Data Preparation Group
- Using Random Sample Tool in Alteryx
**![Random.png](Workflow-Screens/Random.png)**

#### Alteryx Data Preparation Group
- Using Record ID Tool in Alteryx
**![Record ID.png](Workflow-Screens/Record%20ID.png)**

#### Alteryx Reporting Group
- Using Render Tool in Alteryx
**![Render.png](Workflow-Screens/Render.png)**

#### Alteryx Reporting Group
- Using Report Map Tool in Alteryx
**![ReportMap.png](Workflow-Screens/ReportMap.png)**

#### Alteryx Reporting Group
- Using Report Text Tool in Alteryx
**![ReportText.png](Workflow-Screens/ReportText.png)**

**[RunningTotal.png](Workflow-Screens/RunningTotal.png)**
- Alteryx Transformation Group
- Using Running Total Tool in Alteryx

**[Select.png](Workflow-Screens/Select.png)**
- Alteryx Data Preparation Group
- Using Select Tool in Alteryx

**[SelectDynamic.png](Workflow-Screens/SelectDynamic.png)**
- Alteryx Developer Tool Group
- Using Dynamic Select Tool in Alteryx

**[Sort.png](Workflow-Screens/Sort.png)**
- Alteryx Data Preparation Group
- Using Sort Tool in Alteryx

**[Spearman Tool](Workflow-Screens/Spearman.png)**
- Alteryx Data Investigation Group
- Using Spearman Correlation Tool in Alteryx

**[Summarize Tool](Workflow-Screens/Summarize.png)**
- Alteryx Transformation Group
- Using Summarize Tool in Alteryx

**[Table.png](Workflow-Screens/Table.png)**
- Alteryx Reporting Group
- Using Table Tool in Alteryx

**[UnionTool.png](Workflow-Screens/UnionTool.png)**
- Alteryx Join Tool Group
- Using Union Tool in Alteryx

## Disclaimer
The images used in this README are the property of Alteryx, Inc. and are used here for informational purposes only. All rights to these images are retained by Alteryx, Inc. No copyright infringement is intended.
