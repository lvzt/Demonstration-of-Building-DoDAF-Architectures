# A Demonstration of Modeling DoDAF Compliant Architectures Using IBM Rational Rhapsody<br/>
## Contents<br/>
### [Acknowledge](/README.md#acknowledge-1)<br/>
### [1	Introduction](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures/blob/main/README.md#1introduction-1)<br/>
### [2	Modeling demonstration]()<br/>
### [2.1	Modeling process description]()<br/>
### [2.2	Modeling process details]()<br/>
### [2.2.1	Start a project]()<br/>
### [2.2.1.1	Create a new project]()<br/>
### [2.2.1.2	View project structure]()<br/>
### [2.2.2	Build Capability Viewpoint (CV)]()<br/>
### [2.2.2.1	Create CV-2: Capability Taxonomy]()<br/>
### [2.2.2.2	Create CV-4: Capability Dependencies]()<br/>
### [2.2.3	Build Operational Viewpoint (OV)]()<br/>
### [2.2.3.1	Create OV-1: High-Level Operational Concept Graphic]()<br/>
### [2.2.3.2	Create OV-2: Operational Resource Flow Description]()<br/>
### [2.2.3.3	Create OV-5a: Operational Activity Decomposition Tree]()<br/>
### [2.2.3.4	Create OV-5b: Operational Activity Model]()<br/>
### [2.2.3.5	Create OV-6c: Event-Trace Description]()<br/>
### [2.2.3.6	Create Interfaces]()<br/>
### [2.2.3.7	Create OV-2(IBD): Operational Resource Flow Description]()<br/>
### [2.2.3.8	Create OV-6b: State Transition Description]()<br/>
### [2.2.4	Configure component and execute model]()<br/>
### [2.2.4.1	Configure Scope]()<br/>
### [2.2.4.2	Configure Initialization]()<br/>
### [2.2.4.3	Configure Settings]()<br/>
### [2.2.4.4	Execute model]()<br/>
### [2.2.5	Build System Viewpoint (SV)]()<br/>
### [2.2.5.1	Create SV-1: Systems Interface Description]()<br/>
### [2.2.5.2	Create SV-4: Systems Functionality Description]()<br/>
### [2.2.5.3	Create SV-10c: Systems Event-Trace Description]()<br/>
### [2.2.5.4	Create Interfaces]()<br/>
### [2.2.5.5	Create SV-1 (IBD):  Systems Interface Description]()<br/>
### [2.2.5.6	Create SV-10b: Systems State Transition Description]()<br/>
### [2.2.6	Build interdependent viewpoint]()<br/>
### [2.2.6.1	Create SV-5a: Operational Activity to Systems Function Traceability Matrix]()<br/>
### [2.2.6.2	Create SV-5b: Operational Activity to Systems Traceability Matrix]()<br/>
### [3	Integrated scenario demonstration with UE4 (Additional)]()<br/>
<br/><br/>
<br/><br/>

## Acknowledge<br/>
###
This demonstration article by Mr. Zhentao Lu is licensed under [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
<br/>

## 1	Introduction<br/>
###
This demonstration is going to show how to use IBM Rational Rhapsody software to build a DoDAF model.
Note: This demonstration is NOT a mandatary or standard modeling method. Instead, it could be reference way. Because of the feature of DoDAF, any viewpoint or even diagram could be the starting point of modeling.
<br/>
 
(Reference: https://www.visual-paradigm.com/guide/enterprise-architecture/what-is-dodaf-framework/)

For detailed information of DoDAF, go to the websit of Department of Defense.
<br/><br/>
In this demonstration, only Capability Viewpoint (CV), Operational Viewpoint (OV) and Systems Viewpoint (SV) are covered.
<br/><br/>
Computer environment: Windows 10 64-bit
<br/>
Software: IBM Rational Rhapsody 9.0 64-bit, Cygwin 64-bit (When installing Cygwin, remember select gcc-core 、gcc-g++ 、gdb and make under Devel package.)
<br/>
*Note: Visual Studio 2017 Community edition is tested and it works good with Rhapsody.*
<br/>
## 2	Modeling demonstration<br/>
## 2.1	Modeling process description<br/>
###
Repeat again: This process is **NOT** a mandatary or standard modeling method.
<br/>
This demonstration begins with Capability Viewpoint (CV). Then Operational Viewpoint and System Viewpoint are completed.
<br/>
SysML is used for modeling.
<br/>
Activity Diagram (AD) can be introduced for OV-5b and SV-4, Sequence Diagram (ScSD) for OV-6c and SV-10c, and State Diagram for OV-6b and SV-10b, as they are defined in SysML specification to build model from behavior aspect. Both Internal Block Diagram (IBD) and Block Definition Diagram (BDD) can be introduced for OV-2 and SV-1, as they are defined in SysML specification to build model from structure aspect.
<br/>
## 2.2	Modeling process details<br/>
## 2.2.1	Start a project<br/>
## 2.2.1.1	Create a new project<br/>
###
1.	Start Rational Rhapsody 9.0<br/>
2.	Click the **File** on the menu and select **New**<br/>
3.	Fill a project name in **Project name**<br/>
4.	Click **Browse** and browse to the folder E:\IBMworkspace<br/>
5.	In **Project Type** select **UPDM2_DoDAF**<br/>
6.	In **Project Settings** select **SysMLPerspectives**<br/>
7.	Click **OK**<br/>
8.	Click **OK** when a note saying **Directory does not exist** is displayed<br/>
<br/><br/>
2.2.1.2	View project structure
1.	Packages for 8 viewpoints are created. All is empty but All Viewpoint.
 

2.	Double click the Overview of the default architecture structure.
 
3.	View and change the content.
 
By default, packages for all viewpoints are created and brief descriptions are added. For more detailed information about All Viewpoint, go to the website of Department of Defense.
2.2.2	Build Capability Viewpoint (CV)
For more detailed information about Capability Viewpoint, go to the website of Department of Defense.
2.2.2.1	Create CV-2: Capability Taxonomy
For more detailed information about CV-2: Capability Taxonomy, go to the website of Department of Defense.
1.	Right click on CapabilityViewPkg, select Add New -> Capability View Products -> CV-2 Capability Taxonomy
 
2.	Fill in a name for the diagram and click OK
 
3.	Select Capability tool  
4.	Draw a Capability on the diagram
 
5.	Right click the Capability and select Features…
6.	Fill in a name for this Capability
 
Note: Space and “-“ are highly NOT recommended to be included in any names of elements on the diagram.
7.	Add three more Capability elements
 
Tip: When drawing diagrams, Stamp Mode  tool can be pushed down then the item will not be released after clicking it from the panel so the selected item can be added more than once.
8.	Change the name of all those three Capability elements
 
9.	Click   tool then add the relation between the main element and sub-elements
 
10.	 (optional) If names of both ends need to be hided, select the line then right click on the line and choose Display Options…
 
11.	 (optional) De-select all items in the list of End1: Transportation_capability and all items in the list of end2
 
 
2.2.2.2	Create CV-4: Capability Dependencies
For more detailed information about CV-4: Capability Dependencies, go to the website of Department of Defense.
1.	Right click on CapabilityViewPkg, select Add New -> Capability View Products -> CV-4 Capability Taxonomy
 
2.	Fill in a name for the diagram and click OK
 
3.	Expand Capabilities and press Ctrl then select Punctuality and Rapidness
 
4.	Drag Punctuality and Rapidness on the diagram
 
5.	By default the perspective is in Getting Started, so some items on drawing panel are not displayed, to show more drawing items click the perspective list and select Basic
 
Note: the perspective panel is on the upper left.
6.	Click  on the Diagram Tools then connect Punctuality with Rapidness
 
2.2.3	Build Operational Viewpoint (OV)
For more detailed information about Operational Viewpoint, go to the website of Department of Defense.
2.2.3.1	Create OV-1: High-Level Operational Concept Graphic
For more detailed information about OV-1: High-Level Operational Concept Graphic, go to the website of Department of Defense.
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-1 High Level Operational Concept
 
2.	Fill in a name for the diagram and click OK
 
3.	Click   on Diagram Tools then add a high level operational concept on panel
 
4.	Right-click the high level operational concept and select Features…
 
5.	Fill in a name for the high level operational concept and click OK
 
 
6.	Right-click City_Transportation and select Display Options…
 
7.	Click Layout & Image label and check Include Image under Layout
 
8.	Select Image Only and click   in Image Path: then choose a picture


2.2.3.2	Create OV-2: Operational Resource Flow Description
For more detailed information about OV-2: Operational Resource Flow Description, go to the website of Department of Defense.
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-2 Operational Resource Flow Description BDD
 
2.	Fill in a name for the diagram and click OK
 
3.	Click   on Diagram Tools then add a logical architecture on panel
 
4.	Right-click logical architecture and select Features…
 
5.	Fill in a name for logical architecture and click OK
 
 
6.	Click   on Diagram Tools and add four Performer elements
 
7.	Change the name of all those four Performer elements
 
8.	Click   tool then add the relation between the logical architecture and performers
 
Note: The process to hide the information shown on both ends of Composition line is described in CV-2 (2.2.2 A) step 10 and 11.
2.2.3.3	Create OV-5a: Operational Activity Decomposition Tree
For more detailed information about OV-5a: Operational Activity Decomposition Tree, go to the website of Department of Defense.
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-5a Operational Activity Hierarchy
 
2.	Fill in a name for the diagram and click OK
 
3.	Click   on Diagram Tools then add an operational activity on panel
 
4.	Right-click logical architecture and select Features…
 
5.	Fill in a name for operational activity and click OK
 
 
6.	Expand Performer package then drag Ground_transportation on the panel
 
7.	Click   on Diagram Tools then add relationship between performer and operational activity
 
8.	Add two more operational activities then connect them with performer
 
Note: The process to hide the information shown on both ends of Composition line is described in CV-2 (2.2.2 A) step 10 and 11.
2.2.3.4	Create OV-5b: Operational Activity Model
For more detailed information about OV-5b: Operational Activity Model, go to the website of Department of Defense.
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-5b Operational Activity Model
 
2.	Expand ov-5b operational activity model package then double-click OV-5bOperationalActivityModelDiagram
 
3.	Click   on Diagram Tools then add Swimlane Frame on panel
 
4.	Click   on Diagram Tools then add swimlane on panel
 
5.	Drag People from Performers and drop on the title of the swinlane 
 
Note: If the performer is dropped on the diagram, it can be deleted (from view).
6.	Add two more swimlanes and drag all other three performers(Ground_transportation, Aerial_transportation and Railway_transportation) on the title of swimlanes
 
7.	Click   on Diagram Tools then add operational activity actions on panel
 
8.	Right-click operational activity action and select Features…
 
9.	Fill in a name for operational activity action and click OK
 
10.	Click   on Diagram Tools then add initial flow on panel and connect with Set_out action
 
11.	Add more operational activity action and other needed items to complete the diagram. OperationalActivityEdge    is used to connect operational activity actions.
 
Note: If the swinlane frame is too small, press Alt and right-click mouse to expand it.
12.	 Right-click on empty place of diagram (please note do not select any items on diagram) and select UPDM Toolkit -> Create Activities For ActionsCommand
 
13.	Wait for few seconds then result is displayed in Log window
 
14.	Expand OperationalActivities to check all activities created from the diagram
 
2.2.3.5	Create OV-6c: Event-Trace Description
For more detailed information about OV-6c: Event-Trace Description, go to the website of Department of Defense.
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-6c Event Trace Description
 
2.	Fill in a name for the diagram and click OK
 
3.	Expand Performers then each performer on the diagram
 
4.	Click   on Diagram Tools then add operational messages on the lifeline and change the name of messages according to OV-5b
 
5.	Add operational message between lifelines and change the name of messages and change the name
 
6.	Right-click the message reqGround_stop then click Features…
 
7.	Change Message Type from Operation to Event then click OK
 
8.	Complete diagram according to OV-5b: Operational Activity Model
 
9.	Right-click on empty place of diagram (please note do not select any items on diagram) and select Auto Realize all elements
 
10.	New events are created under Event and new operations are created under each performers
 
 
2.2.3.6	Create Interfaces
Note: The Interface is not included in DoDAF. However, it’s critical for passing the events created in previous step (OV-6c) between nodes. In addition, all interfaces have to be attached on ports which can be added in next step (OV-2 (IBD)). All interfaces are direction related so usually the format is Sender_Receiver.
1.	Click the perspective list and select Advanced
 
Note: the perspective panel is on the upper left.
2.	Right click on OperationalViewPkg, select Add New -> Blocks -> Interface
 
3.	Open ov-6c event trace description_transportation and find the first event reqGround_stop() because the event is sent from People to Ground_transportation then change the interface name to People_ Ground_transportation
 
4.	Right-click the event reqGround_stop() then click Navigate -> Locate in Browser
 
5.	The event reqGround_stop() can be found in left tree. Drag this event to People_ Ground_transportation interface
 
 
6.	When drop the event to the interface, a notice is shown and click OK then a new reception is create under the interface
 
 
7.	According to ov-6c event trace description_transportation then create all other interfaces and corresponding receptions
 
2.2.3.7	Create OV-2(IBD): Operational Resource Flow Description
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-2 Operational Resource Flow Description
 
2.	Fill in a name for the diagram and click OK
 
3.	Expand Logical Architectures -> logicalarchitecture_city_transportation -> NodeRoles and select all nodes which are realized performers
 
4.	Drag all nodes on the diagram and rearrange
 
5.	Click   on Diagram Tools then add Port on the edge of People
 
6.	Right click on port_0, select Features…
 
7.	Change name from port_0 to pGround because this port will connect with that of Ground_transportation node and select Behavior under Attributes then click OK
 
8.	Add a port to Ground_transportation
 
9.	Right click port_3 select Features… then change the name to pPeople and select Behavior then click OK
 
10.	Click   on Diagram Tools then connect pPeople on Ground_transportation with pGround on People
 
11.	Right-click pPeople on Ground_transportation then select Features…
 
12.	Click Contract column
 
13.	Click Add in Provided Interfaces
 
14.	 In drop list select People_Ground_transportation then click OK
 
Note: Provided Interfaces contain all events which are provided through the other port by the other performer.
15.	Click Yes when a message is shown to ask for realizing the port
 
16.	Click Add in Required Interfaces
 
17.	In drop list select Ground_transportation_People then click OK
 
Note: Required Interfaces contain all events which are required through current port. Usually, there is no message shown for asking for realizing the port.
18.	Click OK when complete
 
19.	Add Provided Interfaces and Required Interfaces in Contract on pGround port in People node then click OK
 
20.	Add two ports (pRailway and pAerial) in People node, one port (pPeople) in Railway_transportation node and one port (pPeople) in Aerial_transportation node
 
21.	Then add contracts to all other ports
 
 
 
 
22.	(optional) Select all blocks then click   Structured View to change the view of blocks
 
Note: Click one block then press Ctrl + Alt + t so all blocks can be selected.
2.2.3.8	Create OV-6b: State Transition Description
For more detailed information about OV-6b: State Transition Description, go to the website of Department of Defense.
1.	Expand Performers and right-click People performer then click Add New -> Operational View Products -> OV-6b State Transition Description
 
2.	Click   on Diagram Tools then add a state on panel and change the name to Packaging
 
3.	Click   on Diagram Tools then add to Packaging state
 
4.	Add one more state and right-click the state then select Features…
 
5.	Change the name to Walking_on_street and add operation Walk_on_street() in Action on entry then optionally add ; after the operation
 
Note: Ctrl + space can be used to call out a list for selecting all realized operations. But it is not available on Windows 7 because of input system.
6.	(Optional) Press the red circle on Walking_on_street state then show the operation in the state
 
7.	Connect two states with transition
 
Note: Line shape can be changed by right-clicking the transition and select Line Shape -> Rectilinear. To change the default line shape, go to step 24 - 28.
8.	Right click the transition between Packaging and Walking_on_street then select Features…
 
9.	Type in tm(1000) in Trigger and press Enter on keyboard and type in Set_out(); in Action then click OK
 
Note: tm is internal function which means time delay, and the unit is millisecond.
10.	Add one more state then change the name to Waiting and add Wait(); in Action on Entry then add transition between Walking_on_street and Waiting then add Get_to_place(); action in transition
 
11.	Click   on Diagram Tools then add to panel
 
12.	Right-click send action then select Features…
 
13.	Change name to sendreq_Ground_transportation and select pGround in Target and reqGround_stop in Event
 
14.	Expand Packages then right-click BlockModeling and select Add New -> SysML -> ValueProperty
 
15.	Drag the value property to People performer
 
16.	Right-click valueproperty_0 then select Features…
 
17.	Change name to SendReq_Ground_stop and change Type to bool and fill false in Initial Value then click OK
 
18.	Add transition from Waiting to sendreq_Ground_transportation then add !SendReq_Ground_stop in Guard
 
19.	Add transition from sendreq_Ground_transportation to Waiting then add setSendReq_Ground_stop(true); in Action
 
Note: Set a value to indicate whether the event is sent to other performer, and the event is only sent once.
20.	According to OV-5b and OV-6c then complete the OV-6b for People performer
 
21.	According to OV-5b and OV-6c complete OV-6b for Aerial_transportation performer
 
22.	According to OV-5b and OV-6c complete OV-6b for Ground_transportation performer
 
Note: The Condition connector   is not shown on tool panel under Rhapsody 9.0. But this item can be copied from other project and paste to current and there is not problem during compiling.
23.	According to OV-5b and OV-6c complete OV-6b for Railway_transportation performer
 
24.	(Optional) To change the default transition line shape for OV-6b, right-click project root TransportationSoS then select Features…
 
25.	(Optional) Select Properties and click View Common then select All
 
26.	(Optional) Expand StatechartDiagram
 
27.	(Optional) Expand Default Transition then change line_style to rectilinear_arrows
 
28.	 (Optional) Expand Transition then change line_style to rectilinear_arrows then click OK
 
2.2.4	Configure component and execute model
2.2.4.1	Configure Scope
1.	Expand TransportationSoS - > Components and right-click DefaultComponent then select Features…
 
2.	Select Scope
 
3.	Select Selected Elements then select OperationalViewPkg then click OK
 
2.2.4.2	Configure Initialization
1.	Expand TransportationSoS - > Components -> Configurations and right-click DefaultConfig then select Features…
 
2.	Select Initialization
 
3.	Select DoDAD20_Architecture -> OperationalViewPkg -> logicalarchitecture_city_transportation then click Apply
 
2.2.4.3	Configure Settings
1.	On previous window, select Settings
 
2.	Select Animation in Instrumentation Mode
 
3.	(optional) Select correct compiling environment in Environment Settings -> Environment
 
4.	Select Web Enabling then click OK
 
5.	Select Selected Elements then select OperationalViewPkg then click OK
2.2.4.4	Execute model
1.	Click button Generate/Make/Run
 
2.	Click Yes when a message is shown
 
3.	Click Go Action to start animation
 
Note:After clicking Go Action button, all animated state diagrams are activated and stop at first action. Usually, Go button   can be used for activating all state diagrams without stop.
4.	After animation of all performers are shown, click Window then select Tile Horizontally to place all windows
 
5.	Debug the model
 
2.2.5	Build System Viewpoint (SV)
For more detailed information about System Viewpoint, go to the website of Department of Defense.
2.2.5.1	Create SV-1: Systems Interface Description
For more detailed information about SV-1: Systems Interface Description, go to the website of Department of Defense.
Follow the process 2.2.3 B. Create OV-2: Operational Resource Flow Description.
 
2.2.5.2	Create SV-4: Systems Functionality Description
For more detailed information about SV-4: Systems Functionality Description, go to the website of Department of Defense.
Follow the process 2.2.3 D. Create OV-5b: Operational Activity Model.
 
2.2.5.3	Create SV-10c: Systems Event-Trace Description
For more detailed information about SV-10c: Systems Event-Trace Description, go to the website of Department of Defense.
Follow the process 2.2.3 E. Create OV-6c: Event-Trace Description.
(Diagram is omitted.)
2.2.5.4	Create Interfaces
Follow the process 2.2.3 F. Create Interfaces.
(Diagram is omitted.)
2.2.5.5	Create SV-1 (IBD):  Systems Interface Description
Follow the process 2.2.3 G. Create OV-2(IBD): Operational Resource Flow Description.
(Diagram is omitted.)
2.2.5.6	Create SV-10b: Systems State Transition Description
For more detailed information about SV-10b: Systems State Transition Description, go to the website of Department of Defense.
Follow the process 2.2.3 H. Create OV-6b: State Transition Description.
(Diagram is omitted.)
2.2.6	Build interdependent viewpoint
2.2.6.1	Create SV-5a: Operational Activity to Systems Function Traceability Matrix
For more detailed information about SV-5a: Operational Activity to Systems Function Traceability Matrix, go to the website of Department of Defense.
1.	Right click on SystemViewPkg, select Add New -> System View Products -> SV-5a Operational Activity to Systems Function Traceability Matrix
 
2.	Fill in a name (sv-5a operational activity to systems function traceability matrix) for the matrix and right-click the matrix then select Features…
 
3.	Select SystemViewPkg in DoDAF20_Architecture in “From” Scope
 
4.	Select OperationalViewPkg in DoDAF20_Architecture in “To” Scope then click OK
 
5.	Double-click sv-5a operational activity to systems function traceability matrix to open the matrix
 
6.	If any changes are made, Refresh on tool panel can be used to update the matrix. Switch Rows and Columns can be used to transpose the matrix.
 
7.	Right-click the correct cell and select Add New -> Implements to add relationship between operational activity and system function
 
Note: Shift and Ctrl can be used for selecting multipal cells.
2.2.6.2	Create SV-5b: Operational Activity to Systems Traceability Matrix
For more detailed information about SV-5b: Operational Activity to Systems Traceability Matrix, go to the website of Department of Defense.
1.	Right click on SystemViewPkg, select Add New -> System View Products -> SV-5b Operational Activity to Systems Traceability Matrix
 
2.	Fill in a name (sv-5b operational activity to systems traceability matrix) for the matrix and right-click the matrix then select Features…
 
3.	Select SystemViewPkg in DoDAF20_Architecture in “From” Scope
 
4.	Select OperationalViewPkg in DoDAF20_Architecture in “To” Scope then click OK
 
5.	Double-click sv-5b operational activity to systems traceability matrix to open the matrix
 
6.	Press Switch Rows and Columns to transpose the matrix
 
7.	Right-click the correct cell and select Add New -> Implements to add relationship between operational activity and system function
 
3	Integrated scenario demonstration with UE4 (Additional)
In this section an integrated scenario is demonstrated. The model built in IBM Rational Rhapsody is modified and UDP module is added. Commands are sent from the model in Rhapsody then characters in Unreal Engine 4 (UE4) respond after receiving those commands. When the characters finish their actions in UE4, a message will be sent back to Rhapsody which causes state transition or further operation.
Video is posted on YouTube website ().
大陆地区用户可以前往优酷网站浏览（）。

