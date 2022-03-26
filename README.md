# A Demonstration of Modeling DoDAF Compliant Architectures Using IBM Rational Rhapsody<br/>
## Contents<br/>
### [Acknowledge](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#acknowledge-1)<br/>
### [1 Introduction](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#1introduction)<br/>
### [2 Modeling demonstration](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2modeling-demonstration)<br/>
### [2.1 Modeling process description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#21modeling-process-description)<br/>
### [2.2 Modeling process details](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#22modeling-process-details)<br/>
### [2.2.1 Start a project](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#221start-a-project)<br/>
### [2.2.1.1 Create a new project](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2211create-a-new-project)<br/>
### [2.2.1.2 View project structure](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2212view-project-structure)<br/>
### [2.2.2 Build Capability Viewpoint (CV)](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#222build-capability-viewpoint-cv)<br/>
### [2.2.2.1 Create CV 2: Capability Taxonomy](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2221create-cv-2-capability-taxonomy)<br/>
### [2.2.2.2 Create CV 4: Capability Dependencies](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2222create-cv-4-capability-dependencies)<br/>
### [2.2.3 Build Operational Viewpoint (OV)](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#223build-operational-viewpoint-ov)<br/>
### [2.2.3.1 Create OV 1: High Level Operational Concept Graphic](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2231create-ov-1-high-level-operational-concept-graphic)<br/>
### [2.2.3.2 Create OV 2: Operational Resource Flow Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2232create-ov-2-operational-resource-flow-description)<br/>
### [2.2.3.3 Create OV 5a: Operational Activity Decomposition Tree](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2233create-ov-5a-operational-activity-decomposition-tree)<br/>
### [2.2.3.4 Create OV 5b: Operational Activity Model](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2234create-ov-5b-operational-activity-model)<br/>
### [2.2.3.5 Create OV 6c: Event Trace Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2235create-ov-6c-event-trace-description)<br/>
### [2.2.3.6 Create Interfaces](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2236create-interfaces)<br/>
### [2.2.3.7 Create OV 2(IBD): Operational Resource Flow Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2237create-ov-2ibd-operational-resource-flow-description)<br/>
### [2.2.3.8 Create OV 6b: State Transition Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2238create-ov-6b-state-transition-description)<br/>
### [2.2.4 Configure component and execute model](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#224configure-component-and-execute-model)<br/>
### [2.2.4.1 Configure Scope](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2241configure-scope)<br/>
### [2.2.4.2 Configure Initialization](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2242configure-initialization)<br/>
### [2.2.4.3 Configure Settings](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2243configure-settings)<br/>
### [2.2.4.4 Execute model](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2244execute-model)<br/>
### [2.2.5 Build System Viewpoint (SV)](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#225build-system-viewpoint-sv)<br/>
### [2.2.5.1 Create SV 1: Systems Interface Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2251create-sv-1-systems-interface-description)<br/>
### [2.2.5.2 Create SV 4: Systems Functionality Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2252create-sv-4-systems-functionality-description)<br/>
### [2.2.5.3 Create SV 10c: Systems Event Trace Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2253create-sv-10c-systems-event-trace-description)<br/>
### [2.2.5.4 Create Interfaces](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2254create-interfaces)<br/>
### [2.2.5.5 Create SV 1 (IBD):  Systems Interface Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2255create-sv-1-ibd--systems-interface-description)<br/>
### [2.2.5.6 Create SV 10b: Systems State Transition Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2256create-sv-10b-systems-state-transition-description)<br/>
### [2.2.6 Build interdependent viewpoint](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#226build-interdependent-viewpoint)<br/>
### [2.2.6.1 Create SV 5a: Operational Activity to Systems Function Traceability Matrix](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2261create-sv-5a-operational-activity-to-systems-function-traceability-matrix)<br/>
### [2.2.6.2 Create SV 5b: Operational Activity to Systems Traceability Matrix](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2262create-sv-5b-operational-activity-to-systems-traceability-matrix)<br/>
### [3 Integrated scenario demonstration with UE4 (Additional)](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#3integrated-scenario-demonstration-with-ue4-additional)<br/>
<br/><br/>
<br/><br/>

## Acknowledge<br/>
###
This demonstration article by Mr. Zhentao Lu is licensed under [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).<br/>
![](/image/0001%20CC-by.png)
<br/><br/>
Any questions, problems or suggestions are welcome and can be sent by [email](mailto:lvzht@hotmail.com) to the author – Mr. Zhentao Lu.<br/>
<br/><br/>
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
![](/image/22202%20CV-2%20Diagram%20name.jpg)
3.	Select **Capability** ![](/image/22203%20CV-2%20Capability%20tool.jpg) tool on the **Diagram Tools**<br/>
4.	Draw a **Capability** on the diagram<br/>
![](/image/22204%20CV-2%20Capability%20Diagram.jpg)
5.	Right click the **Capability** and select **Features…**<br/>
![](/image/22221%20CV-2%20Capability%20Features.jpg)
7.	Fill in a name for this **Capability**<br/>
![](/image/22205%20CV-2%20Capability%20name.jpg)<br/>
*Note: Space and “-“ are highly NOT recommended to be included in any names of elements on the diagram.*<br/>
7.	Add three more **Capability** elements<br/>
![](/image/22206%20CV-2%20Diagram%20more%20capabilities.jpg)<br/>
*Tip: When drawing diagrams, **Stamp Mode** ![](/image/22207%20CV-2%20Stamp%20Mode.jpg) tool can be pushed down then the item will not be released after clicking it from the panel so the selected item can be added more than once.*<br/>
8.	Change the name of all those three **Capability** elements<br/>
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
3.	Expand **Capabilities** and press **Ctrl** then select **Punctuality** and **Rapidness**<br/>
![](/image/22216%20CV-4%20Drag%20Capability.jpg)
4.	Drag **Punctuality** and **Rapidness** on the diagram<br/>
![](/image/22217%20CV-4%20Diagram.jpg)
5.	By default, the perspective on the top left corn of menu bar is in **Getting Started**, so some items on drawing panel are not displayed, to show more drawing items click the perspective list and select **Basic**<br/>
![](/image/22218%20CV-4%20Change%20Perspective.jpg)
6.	Click **Dependency** ![](/image/22219%20CV-4%20Dependency.jpg) tool on the **Diagram Tools** then connect **Punctuality** with **Rapidness**<br/>
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
8.	Select Image Only and click ![](/image/223110%20OV-1%20Layout%20Image%20browse.jpg) in **Image Path:** then choose a picture and click **Open**<br/>
![](/image/223111%20OV-1%20Image%20open.jpg)
223112 OV-1 Image load ![](/image/223112%20OV-1%20Image%20load.jpg)<br/>
9.	Click **OK**<br/>
![](/image/223113%20OV-1%20Diagram.jpg)<br/>
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
![](/image/223311%20OV-5a%20Diagram%20complete.jpg)<br/>
*Note: The process to hide the information shown on both ends of **Composition** line is described in CV-2 (2.2.2.1) step 10 and 11.*<br/>
## 2.2.3.4	Create OV-5b: Operational Activity Model<br/>
###
For more detailed information about OV-5b: Operational Activity Model, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_ov5ab/) of Department of Defense.<br/>
1.	Right click on **OperationalViewPkg**, select **Add New -> Operational View Products -> OV-5b Operational Activity Model**<br/>
![](/image/223401%20OV-5b%20Create%20Operational%20Activity%20Model.jpg)
2.	Expand **ov-5b operational activity model** package then double-click **OV-5bOperationalActivityModelDiagram**<br/>
![](/image/223402%20OV-5b%20Operational%20Activity%20Model%20name.jpg)
3.	Click **Swimlane Frame** ![](/image/223403%20OV-5b%20Operational%20Activity%20Model%20Swimlane%20Frame.jpg) tool on **Diagram Tools** then add **Swimlane Frame** on panel<br/>
![](/image/223404%20OV-5b%20Operational%20Activity%20Model%20Swimlane%20Frame%20Diagram.jpg)
4.	Click **Swimlane Divider** ![](/image/223405%20OV-5b%20Operational%20Activity%20Model%20Swimlane%20Divider.jpg) tool on **Diagram Tools** then add swimlane divider on the swimlane frame<br/>
![](/image/223406%20OV-5b%20Operational%20Activity%20Model%20Swimlane%20Divider%20Diagram.jpg)
5.	Drag **People** from **Performers** and drop on the title of the swinlane<br/>
![](/image/223420%20OV-5b%20Drag%20Performer.jpg)
![](/image/223421%20OV-5b%20Release%20Performer%20on%20Swimlane%20Title.jpg)
![](/image/223407%20OV-5b%20Operational%20Activity%20Model%20Swimlane%20Performer.jpg)<br/>
*Note: If the performer is dropped on the diagram, it can be deleted (from view)*.<br/>
6.	Add two more swimlanes and drag all other three performers(**Ground_transportation**, **Aerial_transportation** and **Railway_transportation**) on the title of swimlanes<br/>
![](/image/223408%20OV-5b%20Operational%20Activity%20Model%20Swimlane%20Performers.jpg)
7.	Click **OperationalActivityAction** ![](/image/223409%20OV-5b%20Operational%20Activity%20Action.jpg) tool on **Diagram Tools** then add operational activity actions on panel<br/>
![](/image/223410%20OV-5b%20Operational%20Activity%20Action%20Diagram.jpg)
8.	Right-click operational activity action and select **Features…**<br/>
![](/image/223411%20OV-5b%20Operational%20Activity%20Action%20Feature.jpg)
9.	Fill in a name for operational activity action and click **OK**<br/>
![](/image/223412%20OV-5b%20Operational%20Activity%20Action%20Feature%20name.jpg)
10.	Click **Initial Flow** ![](/image/223413%20OV-5b%20Initial%20Flow.jpg) tool on **Diagram Tools** then add initial flow on panel and connect with **Set_out** action<br/>
![](/image/223414%20OV-5b%20Operational%20Activity%20with%20Initial%20Flow.jpg)
11.	Add more operational activity action and other needed items to complete the diagram. **OperationalActivityEdge** ![](/image/223415%20OV-5b%20OperationalActivityEdge.jpg) tool is used to connect operational activity actions.<br/>
![](/image/223416%20OV-5b%20Operational%20Activity%20complete.jpg)<br/>
*Note: If the swinlane frame is too small, click the frame and press and hold Alt then use left-button of mouse to expand it.*<br/>
12.	 Right-click on empty place of diagram (please note do not select any items on diagram) and select **UPDM Toolkit -> Create Activities For ActionsCommand**<br/>
![](/image/223417%20OV-5b%20Create%20Activities%20For%20ActionCommand.jpg)<br/>
*Note: After completion of this action, all names and labels of the operational activity action on the diagram are not allowed to be edited. And all labels will be changed as same as the name of operational activity. But operational activities in step 14 are available to be modified. After any modifiction on name or label of operational activity, it can be reflected on the diagram.*<br/>
13.	Wait for few seconds then result is displayed in **Log** window<br/>
![](/image/223418%20OV-5b%20Create%20Activities%20For%20ActionCommand%20result.jpg)
14.	Expand **OperationalActivities** to check all activities created from the diagram<br/>
![](/image/223419%20OV-5b%20Created%20Activities.jpg)
## 2.2.3.5	Create OV-6c: Event-Trace Description<br/>
###
For more detailed information about OV-6c: Event-Trace Description, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_ov6c/) of Department of Defense.<br/>
1.	Right click on **OperationalViewPkg**, select **Add New -> Operational View Products -> OV-6c Event Trace Description**<br/>
![](/image/223501%20OV-6c%20Create.jpg)
2.	Fill in a name for the diagram and click **OK**<br/>
![](/image/223502%20OV-6c%20Diagram%20name.jpg)
3.	Expand **Performers** then drag each performer on the diagram<br/>
![](/image/223503%20OV-6c%20Drag%20Lifeline.jpg)
4.	Click **OperationalMessage** ![](/image/223504%20OV-6c%20Operational%20Message.jpg) tool on **Diagram Tools** then add operational messages on the lifeline and change the name of messages according to OV-5b<br/>
![](/image/223505%20OV-6c%20Operational%20Message%20Diagram.jpg)
5.	Add operational message between lifelines and change the name of messages and change the name<br/>
![](/image/223506%20OV-6c%20Operational%20Message%20and%20Event%20Diagram.jpg)
6.	Right-click the message **reqGround_stop** then click **Features…**<br/>
![](/image/223507%20OV-6c%20Operational%20Message%20Features.jpg)
7.	Change **Message Type** from **Operation** to **Event** then click **OK**<br/>
![](/image/223508%20OV-6c%20Change%20to%20event.jpg)
8.	Complete diagram according to OV-5b: Operational Activity Model<br/>
![](/image/223509%20OV-6c%20Diagram%20complete.jpg)
9.	Right-click on empty place of diagram (please note do not select any items on diagram) and select **Auto Realize all elements**<br/>
![](/image/223510%20OV-6c%20Auto%20Realize%20all%20elements.jpg)
10.	New events are created under **Event** and new operations are created under each performers<br/>
![](/image/223511%20OV-6c%20Realized%20Events.jpg)
![](/image/223512%20OV-6c%20Realized%20Operations.jpg)<br/>
## 2.2.3.6	Create Interfaces<br/>
###
*Note: The Interface is not included in DoDAF. However, it’s critical for passing the events created in previous step (OV-6c) between nodes. In addition, all interfaces have to be attached on ports which can be added in next step (OV-2 (IBD)). All interfaces are direction related so usually the format is Sender_Receiver.*<br/>
1.	Click the perspective list and select **Advanced**<br/>
![](/image/223601%20Interface%20Change%20Perspective.jpg)<br/>
*Note: the perspective panel is on the top left corn of menu bar.*<br/>
2.	Right click on **OperationalViewPkg**, select **Add New -> Blocks -> Interface**<br/>
![](/image/223602%20Interface%20Create%20interface.jpg)
3.	Open **ov-6c event trace description_transportation** and find the first event **reqGround_stop()** because the event is sent from **People** to **Ground_transportation** then change the interface name to **People_ Ground_transportation**<br/>
![](/image/223603%20Interface%20Change%20interface%20name.jpg)
4.	Right-click the event **reqGround_stop()** then click **Navigate -> Locate in Browser**<br/>
![](/image/223604%20Interface%20Navigate%20event.jpg)
5.	The event **reqGround_stop()** can be found in left tree. Drag this event to **People_ Ground_transportation** interface<br/>
![](/image/223605%20Interface%20Select%20event.jpg)
![](/image/223606%20Interface%20Drag%20to%20interface.jpg)
6.	When drop the event to the interface, a notice is shown and click **OK** then a new reception is created under the interface<br/>
![](/image/223607%20Interface%20Reception%20notice.jpg)<br/>
![](/image/223608%20Interface%20Created%20reception.jpg)
7.	According to **ov-6c event trace description_transportation** then create all other interfaces and corresponding receptions<br/>
![](/image/223609%20Interface%20Completed%20all%20receptions.jpg)
## 2.2.3.7	Create OV-2(IBD): Operational Resource Flow Description<br/>
###
1.	Right click on **OperationalViewPkg**, select **Add New -> Operational View Products -> OV-2 Operational Resource Flow Description**<br/>
![](/image/223701%20OV-2%20Create%20IBD.jpg)
2.	Fill in a name for the diagram and click **OK**<br/>
![](/image/223702%20OV-2%20Diagram%20name.jpg)
3.	Expand **Logical Architectures -> logicalarchitecture_city_transportation -> NodeRoles** and select all nodes which are realized performers<br/>
![](/image/223703%20OV-2%20Select%20noderoles.jpg)
4.	Drag all nodes on the diagram and rearrange<br/>
![](/image/223704%20OV-2%20Drag%20noderoles%20on%20diagram.jpg)
5.	Click **Port** ![](/image/223705%20OV-2%20Port%20tool.jpg) tool on **Diagram Tools** then add **Port** on the edge of **People**<br/>
![](/image/223706%20OV-2%20Port%20added%20on%20node.jpg)
6.	Right click on **port_0**, select **Features…**<br/>
![](/image/223707%20OV-2%20Port%20features.jpg)
7.	Change name from **port_0** to **pGround** because this port will connect with that of **Ground_transportation** node and select **Behavior** under **Attributes** then click **OK**<br/>
![](/image/223708%20OV-2%20Change%20port%20name.jpg)
8.	Add a port to **Ground_transportation**<br/>
![](/image/223709%20OV-2%20Add%20another%20port.jpg)
9.	Right click **port_3** select **Features…** then change the name to **pPeople** and select **Behavior** then click **OK**<br/>
![](/image/223710%20OV-2%20Change%20another%20port%20name.jpg)
10.	Click **Needline** ![](/image/223711%20OV-2%20Needline.jpg) tool on **Diagram Tools** then connect **pPeople** on **Ground_transportation** with **pGround** on **People**<br/>
![](/image/223712%20OV-2%20Connect%20needline.jpg)
11.	Right-click **pPeople** on **Ground_transportation** then select **Features…**<br/>
![](/image/223713%20OV-2%20Port%20features.jpg)
12.	Click **Contract** column<br/>
![](/image/223714%20OV-2%20Port%20contract.jpg)
13.	Click **Add** in **Provided Interfaces**<br/>
![](/image/223715%20OV-2%20Port%20add%20provided%20interfaces.jpg)
14.	 In drop list select **People_Ground_transportation** then click **OK**<br/>
![](/image/223716%20OV-2%20Port%20select%20provided%20interfaces.jpg)<br/>
*Note: Provided Interfaces contain all events which are provided through the other port by the other performer.*<br/>
15.	Click **Yes** when a message is shown to ask for realizing the port<br/>
![](/image/223717%20OV-2%20Port%20info%20to%20realize.jpg)
16.	Click **Add** in **Required Interfaces**<br/>
![](/image/223718%20OV-2%20Port%20add%20required%20interface.jpg)
17.	In drop list select **Ground_transportation_People** then click **OK**<br/>
![](/image/223719%20OV-2%20Port%20select%20required%20interfaces.jpg)<br/>
*Note: Required Interfaces contain all events which are required through current port. Usually, there is no message shown for asking for realizing the port.*<br/>
18.	Click **OK** when complete<br/>
![](/image/223720%20OV-2%20Port%20complete.jpg)
19.	Add **Provided Interfaces** and **Required Interfaces** in **Contract** on **pGround** port in **People** node then click **OK**<br/>
![](/image/223721%20OV-2%20Port%20add%20the%20other%20port.jpg)
20.	Add two ports (**pRailway** and **pAerial**) in **People** node, one port (**pPeople**) in **Railway_transportation** node and one port (**pPeople**) in **Aerial_transportation** node<br/>
![](/image/223722%20OV-2%20Diagram%20add%20two%20more%20ports.jpg)
21.	Then add contracts to all other ports<br/>
![](/image/223723%20OV-2%20Port%20create%20the%20third%20port.jpg)
![](/image/223724%20OV-2%20Port%20create%20the%20fourth%20port.jpg)
![](/image/223725%20OV-2%20Port%20create%20new%20port%20on%20the%20third%20node.jpg)
![](/image/223726%20OV-2%20Port%20create%20new%20port%20on%20the%20fourth%20node.jpg)
22.	(optional) Select all blocks then click ![](/image/223727%20OV-2%20Structure%20View.jpg) **Structured View** to change the view of blocks<br/>
![](/image/223728%20OV-2%20Diagram%20complete.jpg)
*Note: Click one block then press Ctrl + Alt + t so all blocks can be selected.*<br/>
## 2.2.3.8	Create OV-6b: State Transition Description<br/>
###
For more detailed information about OV-6b: State Transition Description, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_ov6b/) of Department of Defense.<br/>
1.	Expand Performers and right-click **People** performer then click **Add New -> Operational View Products -> OV-6b State Transition Description**<br/>
![](/image/223801%20OV-6b%20Create%20for%20people.jpg)
2.	Click **OperationalState** ![](/image/223802%20OV-6b%20Operational%20state.jpg) tool on **Diagram Tools** then add a state on panel and change the name to **Packaging**<br/>
![](/image/223803%20OV-6b%20Add%20one%20state.jpg)
3.	Click **Default Transition** ![](/image/223804%20OV-6b%20Default%20transition.jpg) tool on **Diagram Tools** then add on diagram and connect to **Packaging** state<br/>
![](/image/223805%20OV-6b%20Default%20transition%20connect%20state.jpg)
4.	Add one more state and right-click the state then select **Features…**<br/>
![](/image/223806%20OV-6b%20Second%20state%20features.jpg)
5.	Change the name to **Walking_on_street** and add operation **Walk_on_street()** in **Action on entry** then add **;** after the operation<br/>
![](/image/223807%20OV-6b%20Second%20state%20name%20and%20operation.jpg)<br/>
*Note: Ctrl + space can be used to call out a list for selecting all realized operations. But it is not available on Windows 7 because of input system.*<br/>
6.	(Optional) Press the red circle on **Walking_on_street** state then show the operation in the state<br/>
![](/image/223808%20OV-6b%20Second%20state%20show%20operation.jpg)
7.	7.	Click **Transition** ![](/image/223833%20Transition%20tool.jpg) tool on **Diagram Tools** then add to diagram and connect two states with transition<br/>
![](/image/223809%20OV-6b%20Second%20state%20connect%20with%20first%20state.jpg)<br/>
*Note: Line shape can be changed by right-clicking the transition and select **Line Shape -> Rectilinear**. To change the default line shape, go to step 24 - 28.*<br/>
8.	Right click the transition between **Packaging** and **Walking_on_street** then select **Features…**<br/>
![](/image/223810%20OV-6b%20Transition%20feature.jpg)
9.	Type in **tm(1000)** in **Trigger** and press **Enter** on keyboard and type in **Set_out();** in **Action** then click **OK**<br/>
![](/image/223811%20OV-6b%20Transition%20add%20tm%20and%20action.jpg)
*Note: tm() is internal function which means time delay, and the unit is millisecond.*<br/>
10.	Add one more state then change the name to **Waiting** and add **Wait();** in **Action on Entry** then add transition between **Walking_on_street** and **Waiting** then add **Get_to_place();** action in transition<br/>
![](/image/223812%20OV-6b%20Add%20third%20state.jpg)
11.	Click **Send Action** ![](/image/223813%20OV-6b%20Send%20action%20add.jpg) tool on **Diagram Tools** then add to panel<br/>
![](/image/223814%20OV-6b%20Add%20send%20action.jpg)
12.	Right-click send action then select **Features…**<br/>
![](/image/223815%20OV-6b%20Send%20action%20features.jpg)
13.	Change name to **sendreq_Ground_transportation** and select **pGround** in **Target** and **reqGround_stop** in **Event**<br/>
![](/image/223816%20OV-6b%20Send%20action%20name%20port%20event.jpg)
14.	Expand **Packages** then right-click **BlockModeling** and select **Add New -> SysML -> ValueProperty**<br/>
![](/image/223817%20OV-6b%20Value%20property%20create_modify.jpg)
15.	Drag the value property to **People** performer<br/>
![](/image/223818%20OV-6b%20Value%20property%20drag.jpg)<br/>
*Note: In current version of Rhapsody, value property cannot be added directly under Performer in OV or System in SV. This is the reason why it is created in another package and dragged to the right place.*<br/>
16.	Right-click **valueproperty_0** then select **Features…**<br/>
![](/image/223819%20OV-6b%20Value%20property%20features.jpg)
17.	Change name to **SendReq_Ground_stop** and change **Type** to **bool** and fill **false** in **Initial Value** then click **OK**<br/>
![](/image/223820%20OV-6b%20Value%20property%20name%20type%20initial%20value.jpg)
18.	Add transition from **Waiting** to **sendreq_Ground_transportation** then add **!SendReq_Ground_stop** in **Guard**<br/>
![](/image/223834%20Transition%20with%20guard.jpg)
![](/image/223821%20OV-6b%20Add%20transition%20from%20state%20to%20send%20action.jpg)
19.	Add transition from **sendreq_Ground_transportation** to **Waiting** then add **setSendReq_Ground_stop(true);** in **Action**<br/>
![](/image/223835%20Transition%20with%20set%20value.jpg)
![](/image/223822%20OV-6b%20Add%20trasition%20from%20send%20action%20to%20state.jpg)<br/>
*Note: Set a value to indicate whether the event is sent to the other performer, and the event is only sent once.*<br/>
20.	According to OV-5b and OV-6c then complete the OV-6b for **People** performer<br/>
![](/image/223823%20OV-6b%20State%20diagram%20complete%20for%20first%20performer.jpg)
21.	According to OV-5b and OV-6c complete OV-6b for **Aerial_transportation** performer<br/>
![](/image/223824%20OV-6b%20State%20diagram%20complete%20for%20second%20performer.jpg)
22.	According to OV-5b and OV-6c complete OV-6b for **Ground_transportation** performer<br/>
![](/image/223826%20OV-6b%20State%20diagram%20complete%20for%20third%20performer.jpg)<br/>
*Note: The **Condition connector** ![](/image/223825%20OV-6b%20Condition%20connector.jpg) tool is not shown on tool panel under Rhapsody 9.0. But this item can be copied from other project and paste to current diagram and there is not problem during compiling. This problem is fixed in Rhapsody 9.0.1.*<br/>
23.	According to OV-5b and OV-6c complete OV-6b for **Railway_transportation** performer
![](/image/223827%20OV-6b%20State%20diagram%20complete%20for%20fourth%20performer.jpg)
24.	(Optional) To change the default transition line shape for OV-6b, right-click project root **TransportationSoS** then select **Features…**<br/>
![](/image/223828%20OV-6b%20project%20toot%20features.jpg)
25.	(Optional) Select **Properties** and click **View Common** then select **All**<br/>
![](/image/223829%20OV-6b%20Properties.jpg)
26.	(Optional) Expand **StatechartDiagram**<br/>
![](/image/223830%20OV-6b%20Properties%20view%20all.jpg)
27.	(Optional) Expand **Default Transition** then change **line_style** to **rectilinear_arrows**<br/>
![](/image/223831%20OV-6b%20Default%20transition%20line%20style.jpg)
28.	 (Optional) Expand **Transition** then change **line_style** to **rectilinear_arrows** then click **OK**<br/>
![](/image/223832%20OV-6b%20Transition%20line%20style.jpg)
## 2.2.4	Configure component and execute model<br/>
## 2.2.4.1	Configure Scope<br/>
###
1.	Expand **TransportationSoS - > Components** and right-click **DefaultComponent** then select **Features…**<br/>
![](/image/224101%20OV%20Default%20Component.jpg)
2.	Select **Scope**<br/>
![](/image/224102%20OV%20Default%20Component%20scope.jpg)
3.	Select **Selected Elements** then select **OperationalViewPkg** then click **OK**<br/>
![](/image/224103%20OV%20Default%20Component%20selected%20scope.jpg)
## 2.2.4.2	Configure Initialization<br/>
###
1.	Expand **TransportationSoS - > Components -> Configurations** and right-click **DefaultConfig** then select **Features…**<br/>
![](/image/224201%20OV%20DefaultConfig.jpg)
2.	Select **Initialization**<br/>
![](/image/224202%20OV%20DefaultConfig%20Initialization.jpg)
3.	Select **DoDAD20_Architecture -> OperationalViewPkg -> logicalarchitecture_city_transportation** then click **Apply**<br/>
![](/image/224203%20OV%20DefaultConfig%20selected%20Initialization.jpg)
## 2.2.4.3	Configure Settings<br/>
###
1.	On previous window, select **Settings**<br/>
![](/image/224301%20OV%20DefaultConfig%20Settings.jpg)
2.	Select **Animation** in **Instrumentation Mode**<br/>
![](/image/224302%20OV%20DefaultConfig%20Settings%20animation.jpg)
3.	(optional) Select correct compiling environment in **Environment Settings -> Environment**<br/>
![](/image/224303%20OV%20DefaultConfig%20Settings%20environment.jpg)
4.	(optional) Select **Web Enabling** then click **OK**<br/>
![](/image/224304%20OV%20DefaultConfig%20Settings%20web%20enabling.jpg)
## 2.2.4.4	Execute model<br/>
###
1.	Click button **Generate/Make/Run**<br/>
![](/image/224401%20OV%20Generate%20Make%20Run.jpg)
2.	Click **Yes** when a message is shown<br/>
![](/image/224402%20OV%20Create%20directory.jpg)
3.	Click **Go Action** to start animation<br/>
![](/image/224403%20OV%20Animation%20Go%20Action.jpg)<br/>
*Note: After clicking **Go Action** button, all animated state diagrams are activated and stop at first action. Usually, **Go** ![](/image/224404%20OV%20Animation%20Go.jpg) button can be used for activating all state diagrams without stop.*<br/>
4.	After animation of all performers are shown, click **Window** then select **Tile Horizontally** to place all windows in horizontal manner<br/>
![](/image/224405OV%20Animation%20Window%20tile%20horizontally.jpg)
5.	Debug the model<br/>
![](/image/224406%20OV%20Animation%20debug.jpg)
## 2.2.5	Build System Viewpoint (SV)<br/>
###
For more detailed information about System Viewpoint, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_systems/) of Department of Defense.<br/>
## 2.2.5.1	Create SV-1: Systems Interface Description<br/>
###
For more detailed information about SV-1: Systems Interface Description, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_sv1/) of Department of Defense.<br/>
<br/>
Follow the process [2.2.3.2 Create OV-2: Operational Resource Flow Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2232create-ov-2-operational-resource-flow-description).<br/>
![](/image/225101%20SV-1%20System%20Interface%20Diagram.jpg)
## 2.2.5.2	Create SV-4: Systems Functionality Description<br/>
###
For more detailed information about SV-4: Systems Functionality Description, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_sv4/) of Department of Defense.<br/>
<br/>
Follow the process [2.2.3.4 Create OV-5b: Operational Activity Model](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2234create-ov-5b-operational-activity-model).<br/>
![](/image/225102%20SV-4%20System%20Functionality%20Diagram.jpg)
## 2.2.5.3	Create SV-10c: Systems Event-Trace Description<br/>
###
For more detailed information about SV-10c: Systems Event-Trace Description, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_sv10c/) of Department of Defense.<br/>
<br/>
Follow the process [2.2.3.5 Create OV-6c: Event-Trace Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2235create-ov-6c-event-trace-description).<br/>
<br/>
*(Diagram is omitted.)*<br/>
## 2.2.5.4	Create Interfaces<br/>
###
Follow the process [2.2.3.6 Create Interfaces](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2236create-interfaces).<br/>
<br/>
*(Diagram is omitted.)*<br/>
## 2.2.5.5	Create SV-1 (IBD):  Systems Interface Description<br/>
###
Follow the process [2.2.3.7 Create OV-2(IBD): Operational Resource Flow Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2237create-ov-2ibd-operational-resource-flow-description).<br/>
<br/>
*(Diagram is omitted.)*<br/>
## 2.2.5.6	Create SV-10b: Systems State Transition Description<br/>
###
For more detailed information about SV-10b: Systems State Transition Description, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_sv10b/) of Department of Defense.<br/>
<br/>
Follow the process [2.2.3.8 Create OV-6b: State Transition Description](https://github.com/lvzt/Demonstration-of-Building-DoDAF-Architectures#2238create-ov-6b-state-transition-description).<br/>
<br/>
*(Diagram is omitted.)*<br/>
## 2.2.6	Build interdependent viewpoint<br/>
## 2.2.6.1	Create SV-5a: Operational Activity to Systems Function Traceability Matrix<br/>
###
For more detailed information about SV-5a: Operational Activity to Systems Function Traceability Matrix, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_sv5a/) of Department of Defense.<br/>
1.	Right click on **SystemViewPkg**, select **Add New -> System View Products -> SV-5a Operational Activity to Systems Function Traceability Matrix**<br/>
![](/image/226101%20SV-5a%20Create.jpg)
2.	Fill in a name (**sv-5a operational activity to systems function traceability matrix**) for the matrix and right-click the matrix then select **Features…**<br/>
![](/image/226102%20SV-5a%20Features.jpg)
3.	Select **SystemViewPkg in DoDAF20_Architecture** in **“From” Scope**<br/>
![](/image/226103%20SV-5a%20From%20scope.jpg)
4.	Select **OperationalViewPkg in DoDAF20_Architecture** in **“To” Scope** then click **OK**<br/>
![](/image/226104%20SV-5a%20To%20scope.jpg)
5.	Double-click **sv-5a operational activity to systems function traceability matrix** to open the matrix<br/>
![](/image/226105%20SV-5a%20Matrix.jpg)<br/>
*Note: If the table is happenly opened before setting **“From” Scope** and **“To” Scope**, **Refresh** tool can be used to show the content of the table after those settings are completed.*<br/>
6.	If any changes are made, **Refresh** on tool panel can be used to update the matrix. **Switch Rows and Columns** can be used to transpose the matrix.<br/>
![](/image/226106%20SV-5a%20Tool%20panel.jpg)
7.	Right-click the correct cell and select **Add New -> Implements** to add relationship between operational activity and system function<br/>
![](/image/226107%20SV-5a%20Implements.jpg)<br/>
*Note: Shift and Ctrl can be used for selecting multipal cells.*<br/>
## 2.2.6.2	Create SV-5b: Operational Activity to Systems Traceability Matrix<br/>
###
For more detailed information about SV-5b: Operational Activity to Systems Traceability Matrix, go to the [website](https://dodcio.defense.gov/Library/DoD-Architecture-Framework/dodaf20_sv5b/) of Department of Defense.<br/>
1.	Right click on **SystemViewPkg**, select **Add New -> System View Products -> SV-5b Operational Activity to Systems Traceability Matrix**<br/>
![](/image/226201%20SV-5b%20Create.jpg)
2.	Fill in a name (**sv-5b operational activity to systems traceability matrix**) for the matrix and right-click the matrix then select **Features…**<br/>
![](/image/226202%20SV-5b%20Features.jpg)
3.	Select **SystemViewPkg in DoDAF20_Architecture** in **“From” Scope**<br/>
![](/image/226203%20SV-5b%20From%20scope.jpg)
4.	Select **OperationalViewPkg in DoDAF20_Architecture** in **“To” Scope** then click **OK**<br/>
![](/image/226204%20SV-5b%20To%20scope.jpg)
5.	Double-click **sv-5b operational activity to systems traceability matrix** to open the matrix<br/>
![](/image/226205%20SV-5b%20Matrix.jpg)<br/>
*Note: If the table is happenly opened before setting **“From” Scope** and **“To” Scope**, **Refresh** tool can be used to show the content of the table after those settings are completed.*<br/>
6.	Press **Switch Rows and Columns** to transpose the matrix<br/>
![](/image/226206%20SV-5b%20Matrix%20transpose.jpg)
7.	Right-click the correct cell and select **Add New -> Implements** to add relationship between operational activity and system function<br/>
![](/image/226207%20SV-5b%20Implements.jpg)
## 3	Integrated scenario demonstration with UE4 (Additional)<br/>
###
In this section an integrated scenario is demonstrated. The model built in IBM Rational Rhapsody is modified and UDP module is added. Commands are sent from the model in Rhapsody then characters in Unreal Engine 4 (UE4) respond after receiving those commands. When the characters finish their actions in UE4, a message will be sent back to Rhapsody which causes state transition or further operation.<br/>
<br/><br/>
Video is posted on YouTube website ().<br/>
<br/><br/>
大陆地区用户可以前往优酷网站浏览（）。<br/>
