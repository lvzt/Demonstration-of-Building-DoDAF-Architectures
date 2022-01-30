# A Demonstration of Modeling DoDAF Compliant Architectures Using IBM Rational Rhapsody<br/>
## Contents<br/>
### [Acknowledge](/README.md#acknowledge-1)<br/>
### [1 Introduction](/README.md#1introduction)<br/>
### [2 Modeling demonstration](/README.md#2modeling-demonstration)<br/>
### [2.1 Modeling process description](/README.md#21modeling-process-description)<br/>
### [2.2 Modeling process details](/README.md#22modeling-process-details)<br/>
### [2.2.1 Start a project](/README.md#221start-a-project)<br/>
### [2.2.1.1 Create a new project](/README.md#2211create-a-new-project)<br/>
### [2.2.1.2 View project structure](/README.md#2212view-project-structure)<br/>
### [2.2.2 Build Capability Viewpoint (CV)](/README.md#222build-capability-viewpoint-cv)<br/>
### [2.2.2.1 Create CV 2: Capability Taxonomy](/README.md#2221create-cv-2-capability-taxonomy)<br/>
### [2.2.2.2 Create CV 4: Capability Dependencies](/README.md#2222create-cv-4-capability-dependencies)<br/>
### [2.2.3 Build Operational Viewpoint (OV)](/README.md#223build-operational-viewpoint-ov)<br/>
### [2.2.3.1 Create OV 1: High Level Operational Concept Graphic](/README.md#2231create-ov-1-high-level-operational-concept-graphic)<br/>
### [2.2.3.2 Create OV 2: Operational Resource Flow Description](/README.md#2232create-ov-2-operational-resource-flow-description)<br/>
### [2.2.3.3 Create OV 5a: Operational Activity Decomposition Tree](/README.md#2233create-ov-5a-operational-activity-decomposition-tree)<br/>
### [2.2.3.4 Create OV 5b: Operational Activity Model](/README.md#2234create-ov-5b-operational-activity-model)<br/>
### [2.2.3.5 Create OV 6c: Event Trace Description](/README.md#2235create-ov-6c-event-trace-description)<br/>
### [2.2.3.6 Create Interfaces](/README.md#2236create-interfaces)<br/>
### [2.2.3.7 Create OV 2(IBD): Operational Resource Flow Description](/README.md#2237create-ov-2ibd-operational-resource-flow-description)<br/>
### [2.2.3.8 Create OV 6b: State Transition Description](/README.md#2238create-ov-6b-state-transition-description)<br/>
### [2.2.4 Configure component and execute model](/README.md#224configure-component-and-execute-model)<br/>
### [2.2.4.1 Configure Scope](/README.md#2241configure-scope)<br/>
### [2.2.4.2 Configure Initialization](/README.md#2242configure-initialization)<br/>
### [2.2.4.3 Configure Settings](/README.md#2243configure-settings)<br/>
### [2.2.4.4 Execute model](/README.md#2244execute-model)<br/>
### [2.2.5 Build System Viewpoint (SV)](/README.md#225build-system-viewpoint-sv)<br/>
### [2.2.5.1 Create SV 1: Systems Interface Description](/README.md#2251create-sv-1-systems-interface-description)<br/>
### [2.2.5.2 Create SV 4: Systems Functionality Description](/README.md#2252create-sv-4-systems-functionality-description)<br/>
### [2.2.5.3 Create SV 10c: Systems Event Trace Description](/README.md#2253create-sv-10c-systems-event-trace-description)<br/>
### [2.2.5.4 Create Interfaces](/README.md#2254create-interfaces)<br/>
### [2.2.5.5 Create SV 1 (IBD):  Systems Interface Description](/README.md#2255create-sv-1-ibd--systems-interface-description)<br/>
### [2.2.5.6 Create SV 10b: Systems State Transition Description](/README.md#2256create-sv-10b-systems-state-transition-description)<br/>
### [2.2.6 Build interdependent viewpoint](/README.md#226build-interdependent-viewpoint)<br/>
### [2.2.6.1 Create SV 5a: Operational Activity to Systems Function Traceability Matrix](/README.md#2261create-sv-5a-operational-activity-to-systems-function-traceability-matrix)<br/>
### [2.2.6.2 Create SV 5b: Operational Activity to Systems Traceability Matrix](/README.md#2262create-sv-5b-operational-activity-to-systems-traceability-matrix)<br/>
### [3 Integrated scenario demonstration with UE4 (Additional)](/README.md#3integrated-scenario-demonstration-with-ue4-additional)<br/>
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
<br/><br/>
![](/image/1000%20dodaf.png)<br/>
(Reference: https://www.visual-paradigm.com/guide/enterprise-architecture/what-is-dodaf-framework/)
<br/>
For detailed information of DoDAF, go to the [websit](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/) of Department of Defense.
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
Because of the feature of DoDAF, any viewpoint may be the start point. The following figure describes a practical way to produce corresponding artifacts in different viewpoints. Some relationship views, such as: CV-6, SV-5a and SV-5b, rely on the completeness of other views.<br/>
It is necessary and important to mention that this process is NOT a mandatary or standard modeling method.<br/>
![](/image/2101%20DoDAF%20modeling%20process.jpg)
<br/><br/>
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
![](/image/22111%20Start%20Software.jpg)
3.	Click the **File** on the menu and select **New**<br/>
![](/image/22112%20New.jpg)
4.	Fill a project name in **Project name**<br/>
![](/image/22113%20Project%20name.jpg)
6.	Click **Browse** and browse to the folder E:\IBMworkspace<br/>
![](/image/22114%20Project%20folder.jpg)
8.	In **Project Type** select **UPDM2_DoDAF**<br/>
![](/image/22115%20Project%20type.jpg)
10.	(optional) In **Project Settings** select **SysMLPerspectives**<br/>
![](/image/22116%20Project%20settings.jpg)
12.	Click **OK**<br/>
![](/image/22117%20Create%20Project%20complete.jpg)
14.	Click **Yes** when a note saying **Directory does not exist** is displayed<br/>
![](/image/22118%20Create%20Directory.jpg)
<br/><br/>
## 2.2.1.2	View project structure<br/>
###
1.	Packages for 8 viewpoints are created. All is empty but All Viewpoint.<br/>
![](/image/22121%20Project%20Structure.jpg)
2.	Double click the **Overview of the default architecture structure**.<br/>
![](/image/22122%20AV-1%20Title.jpg)
3.	View and change the content.<br/>
![](/image/22123%20AV-1.jpg)
By default, packages for all viewpoints are created and brief descriptions are added. For more detailed information about All Viewpoint, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_all_view/) of Department of Defense.
<br/><br/>
## 2.2.2	Build Capability Viewpoint (CV)<br/>
###
For more detailed information about Capability Viewpoint, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_capability/) of Department of Defense.<br/>
## 2.2.2.1	Create CV-2: Capability Taxonomy<br/>
###
For more detailed information about CV-2: Capability Taxonomy, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_cv2/) of Department of Defense.<br/>
1.	Right click on **CapabilityViewPkg**, select **Add New -> Capability View Products -> CV-2 Capability Taxonomy**<br/>
![](/image/22201%20CV-2%20Create.jpg)
2.	Fill in a name for the diagram and click OK<br/>
DoDAF Demonstration github 20220129
3.	Select **Capability** tool ![](/image/22203%20CV-2%20Capability%20tool.jpg)<br/>
4.	Draw a Capability on the diagram<br/>
![](/image/22204%20CV-2%20Capability%20Diagram.jpg)
5.	Right click the **Capability** and select **Features…**<br/>
![](/image/22221%20CV-2%20Capability%20Features.jpg)
7.	Fill in a name for this **Capability**<br/>
![](/image/22205%20CV-2%20Capability%20name.jpg)<br/>
*Note: Space and “-“ are highly NOT recommended to be included in any names of elements on the diagram.*<br/>
7.	Add three more Capability elements<br/>
![](/image/22206%20CV-2%20Diagram%20more%20capabilities.jpg)<br/>
*Tip: When drawing diagrams, **Stamp Mode** ![](/image/22207%20CV-2%20Stamp%20Mode.jpg) tool can be pushed down then the item will not be released after clicking it from the panel so the selected item can be added more than once.*<br/>
8.	Change the name of all those three Capability elements<br/>
![](/image/22208%20CV-2%20Diagram%20more%20capabilities%20with%20name.jpg)
9.	Click **Composition** ![](/image/22209%20CV-2%20Composition%20tool.jpg) tool then add the relation between the main element and sub-elements<br/>
![](/image/22210%20Capability%20Diagram%20capability%20with%20association.jpg)
10.	 (optional) If names of both ends need to be hided, select the line then right click on the line and choose **Display Options…**<br/>
![](/image/22211%20CV-2%20Display%20Options.jpg)
11.	 (optional) De-select all items in the list of **End1: Transportation_capability** and all items in the list of end2<br/>
![](/image/22212%20CV-2%20Deselect%20items.jpg)
![](/image/22213%20CV-4%20Change%20Perspective%20complete.jpg)<br/>
## 2.2.2.2	Create CV-4: Capability Dependencies<br/>
###
For more detailed information about CV-4: Capability Dependencies, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_cv4/) of Department of Defense.<br/>
1.	Right click on **CapabilityViewPkg**, select **Add New -> Capability View Products -> CV-4 Capability Taxonomy**<br/>
![](/image/22214%20CV-4%20Create.jpg)
2.	Fill in a name for the diagram and click **OK**<br/>
![](/image/22215%20CV-4%20Diagram%20name.jpg)
3.	Expand **Capabilities** and press Ctrl then select **Punctuality** and **Rapidness**<br/>
![](/image/22216%20CV-4%20Drag%20Capability.jpg)
4.	Drag **Punctuality** and **Rapidness** on the diagram<br/>
![](/image/22217%20CV-4%20Diagram.jpg)
5.	By default, the perspective is in **Getting Started**, so some items on drawing panel are not displayed, to show more drawing items click the perspective list and select **Basic**<br/>
![](/image/22218%20CV-4%20Change%20Perspective.jpg)
6.	Click **Dependency** ![](/image/22219%20CV-4%20Dependency.jpg) tool on the Diagram Tools then connect **Punctuality** with **Rapidness**<br/>
![](/image/22220%20CV-4%20Diagram%20with%20dependency.jpg)<br/>
## 2.2.3	Build Operational Viewpoint (OV)<br/>
For more detailed information about Operational Viewpoint, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_operational/) of Department of Defense.<br/>
## 2.2.3.1	Create OV-1: High-Level Operational Concept Graphic<br/>
###
For more detailed information about OV-1: High-Level Operational Concept Graphic, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_ov1/) of Department of Defense.<br/>
1.	Right click on **OperationalViewPkg**, select **Add New -> Operational View Products -> OV-1 High Level Operational Concept**<br/>
![](/image/223101%20OV-1%20Create.jpg)
2.	Fill in a name for the diagram and click **OK**<br/>
![](/image/223102%20OV-1%20Diagram%20name.jpg)
3.	Click **HighLevelOperationalConcept** ![](/image/223103%20OV-1%20High%20Level%20Operational%20Concept.jpg) tool on **Diagram Tools** then add a high level operational concept on panel<br/>
![](/image/223104%20OV-1%20Diagram%20with%20High%20Level%20Operational%20Concept.jpg)
4.	Right-click the high level operational concept and select **Features…**<br/>
![](/image/223105%20OV-1%20Features.jpg)
5.	Fill in a name for the high level operational concept and click **OK**<br/>
![](/image/223106%20OV-1%20Diagram%20Name.jpg)
![](/image/223107%20OV-1%20Diagram%20Ligh%20level%20Operational%20Concept%20with%20name.jpg)
6.	Right-click **City_Transportation** and select **Display Options…**<br/>
![](/image/223108%20OV-1%20Display%20Options.jpg)
7.	Click **Layout & Image label** and check **Include Image** under **Layout**<br/>
![](/image/223109%20OV-1%20Layout%20Image.jpg)
8.	Select **Image Only** and click ![](/image/223110%20OV-1%20Layout%20Image.jpg) in **Image Path:** then choose a picture<br/>

## 2.2.3.2	Create OV-2: Operational Resource Flow Description<br/>
###
For more detailed information about OV-2: Operational Resource Flow Description, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_ov2/) of Department of Defense.<br/>
1.	Right click on **OperationalViewPkg**, select **Add New -> Operational View Products -> OV-2 Operational Resource Flow Description BDD**<br/>
![](/image/223201%20OV-2%20Create.jpg)
2.	Fill in a name for the diagram and click **OK**<br/>
![](/image/223202%20OV-2%20Diagram%20name.jpg)
3.	Click **LogicalArchitecture** ![](/image/223203%20OV-2%20Logical%20Architecture.jpg) tool on **Diagram Tools** then add a logical architecture on panel<br/>
![](/image/223204%20OV-2%20Diagram%20with%20logicalarchitecture.jpg)
4.	Right-click logical architecture and select **Features…**<br/>
![](/image/223205%20OV-2%20Logical%20Architecture%20features.jpg)
5.	Fill in a name for logical architecture and click **OK**<br/>
![](/image/223206%20OV-2%20Logical%20Architecture%20name.jpg)
6.	Click **Performer** ![](/image/223208%20OV-2%20Performer.jpg) tool on **Diagram Tools** and add four **Performer** elements<br/>
![](/image/223209%20OV-2%20Diagram%20logicalarchitecture%20with%20performer.jpg)
7.	Change the name of all those four **Performer** elements<br/>
![](/image/223210%20OV-2%20Diagram%20performer%20change%20name.jpg)
8.	Click **Composition** ![](/image/223211%20OV-2%20Composition%20tool.jpg) tool then add the relation between the logical architecture and performers<br/>
![](/image/223212%20OV-2%20Diagram%20complete.jpg)<br/>
*Note: The process to hide the information shown on both ends of **Composition** line is described in CV-2 (2.2.2.1) step 10 and 11.*<br/>
## 2.2.3.3	Create OV-5a: Operational Activity Decomposition Tree<br/>
###
For more detailed information about OV-5a: Operational Activity Decomposition Tree, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_ov5ab/) of Department of Defense.<br/>
1.	Right click on **OperationalViewPkg**, select **Add New -> Operational View Products -> OV-5a Operational Activity Hierarchy**<br/>
![](/image/223301%20OV-5a%20Create.jpg)
2.	Fill in a name for the diagram and click **OK**<br/>
![](/image/223302%20OV-5a%20Diagram%20name.jpg)
3.	Click **OperationalActivity** ![](/image/223303%20OV-5a%20Operational%20Activity.jpg) tool on **Diagram Tools** then add an operational activity on panel<br/>
![](/image/223304%20OV-5a%20Diagram%20Operational%20Activity.jpg)
4.	Right-click logical architecture and select **Features…**<br/>
![](/image/223305%20OV-5a%20Features.jpg)
5.	Fill in a name for operational activity and click **OK**<br/>
![](/image/223306%20OV-5a%20Operational%20Activity%20name.jpg)
![](/image/223307%20OV-5a%20Operational%20Activity%20complete.jpg)
6.	Expand **Performer** package then drag **Ground_transportation** on the panel<br/>
![](/image/223308%20OV-5a%20Add%20performer.jpg)
7.	Click **ActivityPerformedByPerformer** ![](/image/223309%20OV-5a%20ActivityPerformedByPerformer.jpg) tool on **Diagram Tools** then add relationship between performer and operational activity<br/>
![](/image/223310%20OV-5a%20Diagram%20Activity%20with%20performer.jpg)
8.	Add two more operational activities then connect them with performer<br/>
![](/image/223311%20OV-5a%20Diagram%20complete.jpg)
*Note: The process to hide the information shown on both ends of **Composition** line is described in CV-2 (2.2.2.1) step 10 and 11.*<br/>
## 2.2.3.4	Create OV-5b: Operational Activity Model<br/>
###
For more detailed information about OV-5b: Operational Activity Model, go to the website of Department of Defense.<br/>
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-5b Operational Activity Model<br/>
 
2.	Expand ov-5b operational activity model package then double-click OV-5bOperationalActivityModelDiagram<br/>
 
3.	Click   on Diagram Tools then add Swimlane Frame on panel<br/>
 
4.	Click   on Diagram Tools then add swimlane on panel<br/>
 
5.	Drag People from Performers and drop on the title of the swinlane<br/>
 
Note: If the performer is dropped on the diagram, it can be deleted (from view).<br/>
6.	Add two more swimlanes and drag all other three performers(Ground_transportation, Aerial_transportation and Railway_transportation) on the title of swimlanes<br/>
 
7.	Click   on Diagram Tools then add operational activity actions on panel<br/>
 
8.	Right-click operational activity action and select Features…<br/>
 
9.	Fill in a name for operational activity action and click OK<br/>
 
10.	Click   on Diagram Tools then add initial flow on panel and connect with Set_out action<br/>
 
11.	Add more operational activity action and other needed items to complete the diagram. OperationalActivityEdge    is used to connect operational activity actions.<br/>
 
Note: If the swinlane frame is too small, press Alt and right-click mouse to expand it.
12.	 Right-click on empty place of diagram (please note do not select any items on diagram) and select UPDM Toolkit -> Create Activities For ActionsCommand<br/>
 
13.	Wait for few seconds then result is displayed in Log window<br/>
 
14.	Expand OperationalActivities to check all activities created from the diagram<br/>
 
## 2.2.3.5	Create OV-6c: Event-Trace Description<br/>
###
For more detailed information about OV-6c: Event-Trace Description, go to the website of Department of Defense.<br/>
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-6c Event Trace Description<br/>
 
2.	Fill in a name for the diagram and click OK<br/>
 
3.	Expand Performers then each performer on the diagram<br/>
 
4.	Click   on Diagram Tools then add operational messages on the lifeline and change the name of messages according to OV-5b<br/>
 
5.	Add operational message between lifelines and change the name of messages and change the name<br/>
 
6.	Right-click the message reqGround_stop then click Features…<br/>
 
7.	Change Message Type from Operation to Event then click OK<br/>
 
8.	Complete diagram according to OV-5b: Operational Activity Model<br/>
 
9.	Right-click on empty place of diagram (please note do not select any items on diagram) and select Auto Realize all elements<br/>
 
10.	New events are created under Event and new operations are created under each performers<br/>
 
## 2.2.3.6	Create Interfaces<br/>
###
Note: The Interface is not included in DoDAF. However, it’s critical for passing the events created in previous step (OV-6c) between nodes. In addition, all interfaces have to be attached on ports which can be added in next step (OV-2 (IBD)). All interfaces are direction related so usually the format is Sender_Receiver.<br/>
1.	Click the perspective list and select Advanced<br/>
 
Note: the perspective panel is on the upper left.<br/>
2.	Right click on OperationalViewPkg, select Add New -> Blocks -> Interface<br/>
 
3.	Open ov-6c event trace description_transportation and find the first event reqGround_stop() because the event is sent from People to Ground_transportation then change the interface name to People_ Ground_transportation<br/>
 
4.	Right-click the event reqGround_stop() then click Navigate -> Locate in Browser<br/>
 
5.	The event reqGround_stop() can be found in left tree. Drag this event to People_ Ground_transportation interface<br/>

6.	When drop the event to the interface, a notice is shown and click OK then a new reception is created under the interface<br/>
 
7.	According to ov-6c event trace description_transportation then create all other interfaces and corresponding receptions<br/>
 
## 2.2.3.7	Create OV-2(IBD): Operational Resource Flow Description<br/>
###
1.	Right click on OperationalViewPkg, select Add New -> Operational View Products -> OV-2 Operational Resource Flow Description<br/>
 
2.	Fill in a name for the diagram and click OK<br/>
 
3.	Expand Logical Architectures -> logicalarchitecture_city_transportation -> NodeRoles and select all nodes which are realized performers<br/>
 
4.	Drag all nodes on the diagram and rearrange<br/>
 
5.	Click   on Diagram Tools then add Port on the edge of People<br/>
 
6.	Right click on port_0, select Features…<br/>
 
7.	Change name from port_0 to pGround because this port will connect with that of Ground_transportation node and select Behavior under Attributes then click OK<br/>
 
8.	Add a port to Ground_transportation<br/>
 
9.	Right click port_3 select Features… then change the name to pPeople and select Behavior then click OK<br/>
 
10.	Click   on Diagram Tools then connect pPeople on Ground_transportation with pGround on People<br/>
 
11.	Right-click pPeople on Ground_transportation then select Features…<br/>
 
12.	Click Contract column<br/>
 
13.	Click Add in Provided Interfaces<br/>
 
14.	 In drop list select People_Ground_transportation then click OK<br/>
 
Note: Provided Interfaces contain all events which are provided through the other port by the other performer.<br/>
15.	Click Yes when a message is shown to ask for realizing the port<br/>
 
16.	Click Add in Required Interfaces<br/>
 
17.	In drop list select Ground_transportation_People then click OK<br/>
 
Note: Required Interfaces contain all events which are required through current port. Usually, there is no message shown for asking for realizing the port.<br/>
18.	Click OK when complete<br/>
 
19.	Add Provided Interfaces and Required Interfaces in Contract on pGround port in People node then click OK<br/>
 
20.	Add two ports (pRailway and pAerial) in People node, one port (pPeople) in Railway_transportation node and one port (pPeople) in Aerial_transportation node<br/>
 
21.	Then add contracts to all other ports<br/>


22.	(optional) Select all blocks then click   Structured View to change the view of blocks<br/>
 
Note: Click one block then press Ctrl + Alt + t so all blocks can be selected.<br/>
## 2.2.3.8	Create OV-6b: State Transition Description<br/>
###
For more detailed information about OV-6b: State Transition Description, go to the website of Department of Defense.<br/>
1.	Expand Performers and right-click People performer then click Add New -> Operational View Products -> OV-6b State Transition Description<br/>
 
2.	Click   on Diagram Tools then add a state on panel and change the name to Packaging<br/>
 
3.	Click   on Diagram Tools then add to Packaging state<br/>
 
4.	Add one more state and right-click the state then select Features…<br/>
 
5.	Change the name to Walking_on_street and add operation Walk_on_street() in Action on entry then optionally add ; after the operation<br/>
 
Note: Ctrl + space can be used to call out a list for selecting all realized operations. But it is not available on Windows 7 because of input system.<br/>
6.	(Optional) Press the red circle on Walking_on_street state then show the operation in the state<br/>
 
7.	Connect two states with transition<br/>
 
Note: Line shape can be changed by right-clicking the transition and select Line Shape -> Rectilinear. To change the default line shape, go to step 24 - 28.<br/>
8.	Right click the transition between Packaging and Walking_on_street then select Features…<br/>
 
9.	Type in tm(1000) in Trigger and press Enter on keyboard and type in Set_out(); in Action then click OK<br/>
 
Note: tm is internal function which means time delay, and the unit is millisecond.<br/>
10.	Add one more state then change the name to Waiting and add Wait(); in Action on Entry then add transition between Walking_on_street and Waiting then add Get_to_place(); action in transition<br/>
 
11.	Click   on Diagram Tools then add to panel<br/>
 
12.	Right-click send action then select Features…<br/>
 
13.	Change name to sendreq_Ground_transportation and select pGround in Target and reqGround_stop in Event<br/>
 
14.	Expand Packages then right-click BlockModeling and select Add New -> SysML -> ValueProperty<br/>
 
15.	Drag the value property to People performer<br/>
 
16.	Right-click valueproperty_0 then select Features…<br/>
 
17.	Change name to SendReq_Ground_stop and change Type to bool and fill false in Initial Value then click OK<br/>
 
18.	Add transition from Waiting to sendreq_Ground_transportation then add !SendReq_Ground_stop in Guard<br/>
 
19.	Add transition from sendreq_Ground_transportation to Waiting then add setSendReq_Ground_stop(true); in Action<br/>
 
Note: Set a value to indicate whether the event is sent to the other performer, and the event is only sent once.<br/>
20.	According to OV-5b and OV-6c then complete the OV-6b for People performer<br/>
 
21.	According to OV-5b and OV-6c complete OV-6b for Aerial_transportation performer<br/>
 
22.	According to OV-5b and OV-6c complete OV-6b for Ground_transportation performer<br/>
 
Note: The Condition connector   is not shown on tool panel under Rhapsody 9.0. But this item can be copied from other project and paste to current and there is not problem during compiling.<br/>
23.	According to OV-5b and OV-6c complete OV-6b for Railway_transportation performer
 
24.	(Optional) To change the default transition line shape for OV-6b, right-click project root TransportationSoS then select Features…<br/>
 
25.	(Optional) Select Properties and click View Common then select All<br/>
 
26.	(Optional) Expand StatechartDiagram<br/>
 
27.	(Optional) Expand Default Transition then change line_style to rectilinear_arrows<br/>
 
28.	 (Optional) Expand Transition then change line_style to rectilinear_arrows then click OK<br/>
 
## 2.2.4	Configure component and execute model<br/>
## 2.2.4.1	Configure Scope<br/>
###
1.	Expand TransportationSoS - > Components and right-click DefaultComponent then select Features…<br/>
 
2.	Select Scope<br/>
 
3.	Select Selected Elements then select OperationalViewPkg then click OK<br/>
 
## 2.2.4.2	Configure Initialization<br/>
###
1.	Expand TransportationSoS - > Components -> Configurations and right-click DefaultConfig then select Features…<br/>
 
2.	Select Initialization<br/>
 
3.	Select DoDAD20_Architecture -> OperationalViewPkg -> logicalarchitecture_city_transportation then click Apply<br/>
 
## 2.2.4.3	Configure Settings<br/>
###
1.	On previous window, select Settings<br/>
 
2.	Select Animation in Instrumentation Mode<br/>
 
3.	(optional) Select correct compiling environment in Environment Settings -> Environment<br/>
 
4.	Select Web Enabling then click OK<br/>
 
5.	Select Selected Elements then select OperationalViewPkg then click OK<br/>
## 2.2.4.4	Execute model<br/>
###
1.	Click button Generate/Make/Run<br/>
 
2.	Click Yes when a message is shown<br/>
 
3.	Click Go Action to start animation<br/>
 
Note:After clicking Go Action button, all animated state diagrams are activated and stop at first action. Usually, Go button   can be used for activating all state diagrams without stop.<br/>
4.	After animation of all performers are shown, click Window then select Tile Horizontally to place all windows<br/>
 
5.	Debug the model<br/>
 
## 2.2.5	Build System Viewpoint (SV)<br/>
###
For more detailed information about System Viewpoint, go to the website of Department of Defense.<br/>
## 2.2.5.1	Create SV-1: Systems Interface Description<br/>
###
For more detailed information about SV-1: Systems Interface Description, go to the website of Department of Defense.<br/>
<br/>
Follow the process 2.2.3 B. Create OV-2: Operational Resource Flow Description.<br/>
 
## 2.2.5.2	Create SV-4: Systems Functionality Description<br/>
###
For more detailed information about SV-4: Systems Functionality Description, go to the website of Department of Defense.<br/>
<br/>
Follow the process 2.2.3 D. Create OV-5b: Operational Activity Model.<br/>
 
## 2.2.5.3	Create SV-10c: Systems Event-Trace Description<br/>
###
For more detailed information about SV-10c: Systems Event-Trace Description, go to the website of Department of Defense.<br/>
<br/>
Follow the process 2.2.3 E. Create OV-6c: Event-Trace Description.<br/>
<br/>
(Diagram is omitted.)<br/>
## 2.2.5.4	Create Interfaces<br/>
###
Follow the process 2.2.3 F. Create Interfaces.<br/>
<br/>
(Diagram is omitted.)<br/>
## 2.2.5.5	Create SV-1 (IBD):  Systems Interface Description<br/>
###
Follow the process 2.2.3 G. Create OV-2(IBD): Operational Resource Flow Description.<br/>
<br/>
(Diagram is omitted.)<br/>
## 2.2.5.6	Create SV-10b: Systems State Transition Description<br/>
###
For more detailed information about SV-10b: Systems State Transition Description, go to the website of Department of Defense.<br/>
<br/>
Follow the process 2.2.3 H. Create OV-6b: State Transition Description.<br/>
<br/>
(Diagram is omitted.)<br/>
## 2.2.6	Build interdependent viewpoint<br/>
## 2.2.6.1	Create SV-5a: Operational Activity to Systems Function Traceability Matrix<br/>
###
For more detailed information about SV-5a: Operational Activity to Systems Function Traceability Matrix, go to the website of Department of Defense.<br/>
1.	Right click on SystemViewPkg, select Add New -> System View Products -> SV-5a Operational Activity to Systems Function Traceability Matrix<br/>
 
2.	Fill in a name (sv-5a operational activity to systems function traceability matrix) for the matrix and right-click the matrix then select Features…<br/>
 
3.	Select SystemViewPkg in DoDAF20_Architecture in “From” Scope<br/>
 
4.	Select OperationalViewPkg in DoDAF20_Architecture in “To” Scope then click OK<br/>
 
5.	Double-click sv-5a operational activity to systems function traceability matrix to open the matrix<br/>
 
6.	If any changes are made, Refresh on tool panel can be used to update the matrix. Switch Rows and Columns can be used to transpose the matrix.<br/>
 
7.	Right-click the correct cell and select Add New -> Implements to add relationship between operational activity and system function<br/>
 
Note: Shift and Ctrl can be used for selecting multipal cells.<br/>
## 2.2.6.2	Create SV-5b: Operational Activity to Systems Traceability Matrix<br/>
###
For more detailed information about SV-5b: Operational Activity to Systems Traceability Matrix, go to the website of Department of Defense.<br/>
1.	Right click on SystemViewPkg, select Add New -> System View Products -> SV-5b Operational Activity to Systems Traceability Matrix<br/>
 
2.	Fill in a name (sv-5b operational activity to systems traceability matrix) for the matrix and right-click the matrix then select Features…<br/>
 
3.	Select SystemViewPkg in DoDAF20_Architecture in “From” Scope<br/>
 
4.	Select OperationalViewPkg in DoDAF20_Architecture in “To” Scope then click OK<br/>
 
5.	Double-click sv-5b operational activity to systems traceability matrix to open the matrix<br/>
 
6.	Press Switch Rows and Columns to transpose the matrix<br/>
 
7.	Right-click the correct cell and select Add New -> Implements to add relationship between operational activity and system function<br/>
 
## 3	Integrated scenario demonstration with UE4 (Additional)<br/>
###
In this section an integrated scenario is demonstrated. The model built in IBM Rational Rhapsody is modified and UDP module is added. Commands are sent from the model in Rhapsody then characters in Unreal Engine 4 (UE4) respond after receiving those commands. When the characters finish their actions in UE4, a message will be sent back to Rhapsody which causes state transition or further operation.<br/>
<br/><br/>
Video is posted on YouTube website ().<br/>
<br/><br/>
大陆地区用户可以前往优酷网站浏览（）。<br/>
