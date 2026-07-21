This repository documents my personal learning journey using Revit LinkedIn Learning courses with the Revit 2027 30 day trial to learn the most recent version of the software.

**Disclaimer**: I do not own the copyright to the course videos or original exercise files. All rights belong to LinkedIn Learning and Eric Wing. All original course materials (videos, exercise files) are copyright of LinkedIn Learning and are not included in this repository. The course is linked below, note that it requires authorization to access via membership.

**Repository Content**: The files in this repository are my own practice drawings and notes created while following the courses. They are shared here to demonstrate my progress and understanding of Revit.

## Revit 2023: Essential Training for MEP
<details>
<summary> 1. Introduction </summary>

  Key Takeaways:
  * Intro to the course and what it will cover. 

<details> 
<summary> Notes </summary>

  The industry has recently standardized to the Revit platform, making it easier for collabration across trades.
  * This means it is imperitave to learn Revit, not only as a building model software but also its collaboration workflows.

  This course will cover how to start a project, then MEP applications, and finally how to extract information and schedules. 
</details>
</details>

<details>
<summary> 2. Starting a Revit Project </summary>

  Key Takeaways:
  * Revit uses templates for projects - different companies typically have their own versions.
  * Electrical model has specific perks when working with electrical drawings, like adding cable trays with fittings.
  * Took a tour of the user interface with the home tab, quick access toolbar, context sensitive menus, and project browser.
  * Learned how to link other Revit models into an Electrical project and used the Pin tool to make sure they cannot accidentally be moved.
  * Learned how to add spaces to a building, edit and transfer names and number properties, and generate a schedule to clean up the spaces in "unoccupied" zones.
  * Learned how to copy levels and ensure they are aligned between architectural and structural, as well as set up monitoring so a warning displays is an architectural level changes.
  * Learned how to create new views with the proper templates and delete no longer needed views in an organized manner. 

<details> 
<summary> Notes </summary>

  **Starting a Project using Revit Templates**
  * Starting with the right template is crucial as the project progresses. Many companies have their own starting templates, for this course we will use the default Revit Electrical Template.
  * I clicked "New" on the Model panel from the home screen and selected the Electrical Default Template.
  * This opened an electrical project, and exploring the Floor Plan - Power drawing we can see the Properties tab shows different aspects.
  * For example, looking at the Systems tab we can add some cable trays and notice that the fittings are automatically inserted as you draw.
    * If you were to do this in say an architectural template, none of this would have happened.
  * Note - similar to AutoCAD, selecting from left to right is the selection tool requiring the entire object to be selected, while clicking from right to left is the partial selection tool where anything in the box will be selected.
  * Holding CTRL you can select items individually.
  * I saved the project and changed the options to have 1 backup instead of 3.


  **Touring the User Interface**
  * The Revit interface is not as customizable as some of the other drafting programs.
  * The home screen lets you open.create new models or families and displays recently opened projects and families.
  * Now opening the Electrical Model we created from the last module.
    * Commonly used icons are up on the quick access toolbar, you can also right click on any icon and add it to the QAT. Clicking on the dropdown lets you add or unadd default ones as well.
    * When you click on an icon in a tab on the ribbon, the interface will change to give you the specific properties of the icon.
      * Companies will likely have their own families loaded into their specific template.
  * In the project browser there are views that will be sorted by discipline.
  * We can also change into a 3D view by clicking on the house icon in the QAT.
  * Seems to have a lot of similar features to AutoCAD, just specific to electrical layouts.

  **Linking Other Models**
  * The first thing that is done at the start of any MEP project is to link other trades in.
  * Going to the insert tab and clicking "Link Revit" and using the course files we can link the "Architectural" drawing.
    * Note - positioning is the important one, generally "Auto - Internal Origin to Internal Origin".
  * I did this with the [Architectural file](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Adding%20Architectural%20Background.png) in the exercises, then pinned it so it cannot be accidentally moved.
  * Then I went into Edit Type on the properties panel and turned on room bounding. Also unchecked select pin elements so it cannot be selected.
  * Then I linked the structural model as well.
  * Note - since I am using the 2027 version, Revit updated the 2023 models to the 2027 versions needed.
  * Then, going into a 3D view we can see the [full building](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Full%20Structure%20(Arch-Struct).png). I made sure everything was pinned by using the selection tool, filtering by Revit Links and clicked the Pin icon.

  **Adding Spaces**
  * Spaces in Revit MEP mimic rooms in Revit Architecture but Spaces allow us to calculate heating and cooling loads and lighting levels.
  * Here we will add spaces, configure space tags, and rename spaces.
  * Opening "Electrical Project Spaces" from the exercise files and in the Power 1 floor plan.
    * Note, once we put a space in, it will be in every view even if in a specific layer (a space is a 3D element).
  * Going to the Analyze tab and clicking space, I [added a space](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Adding%20a%20Space.png) to the lower left room on the right side of the building.
  * I then went in and edited the Space Name, changing it to Room Name, and changed the number from Number to Room Number.
  * I then used the [Place Spaces Automatically](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Adding%20Spaces%20Automatically.png) tool to fill in the [rest of the building](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Added%20Spaces%20in%20Building.png).
  * Now we need to edit some of the automatically filled spaces, best to do this in a schedule so I went to the View tab and into Schedule/Quantities.
  * Going into Spaces and then changing the drop down into "Rooms", adding Room/Space Name and Room/Space Number into the [Scheduled Fields box](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Setting%20Schedule%20Properties.png).
  * Then I filtered by room number to [generate the schedule](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Generated%20Space%20Schedule.png). All the rooms without a Room: Name we can [delete](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Removing%20Redundant%20Spaces.png) as those are "unoccupied".
  * Now we need to fix the labeling, so going into the Analyze tab and Space Naming to [transfer the Room properties](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Transferring%20Room%20Properties.png) to the Number and Name properties.
  * Now the [redundant spaces are gone](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Spaces%20in%20Building%20%20after%20Removal.png) in our full building layout.


  **Copying Levels and Setting Up Monitoring**
  * The Architectural and Structural models have a lot of underlays and grids, but in our current model we only have 2.
  * We can copy the levels from the architectural model and the grids from the structural model.
  * But, we can copy them in such a way that it keeps a "live model" - so if the architect moves a level or grid, we get a coordination alert.
  * Used the "tag all" button in Analyze to add the previously made space tags into the rooms again.
  * Went into the "South Elevations" in the Project Browser and went into Visibility/Graphics to change the structural linked view to change the Display Settings to "custom" and uncheck the "show categories" in the annotations tab.
    * This eliminated the "duplicate" level tags in the Elevation View.
  * Now we would like to [align the structural Level 2 with the Architectural Level 2](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Align%20L2.png).
  * On Modify Tab, click "Align" - then click the level you want to align TO first, then the level to [bring into alignment](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Aligned%20L2.png).
  * For the rest of the levels, we can "copy monitor" the rest of them on the collaborate tab.
  * Using select link, [selecting the architectural](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Selecting%20Arch%20Model.png), then Copy/Monitor, Copy, Copy multiple and CTRL selecting Level 4, 5, and Roof, then hitting "finish".
  * Back to the 1 - Lighting to repeat the process with the [structural model](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Copy%20and%20Monitor%20Struct.png) with the gridlines. 


  **Creating Floor Plans**
  * Objective here is to add views to the project browser and duplicate existing views.
  * Going to the "view" tab, clicking "plan views" and "floor plan". Here, we only see levels 3-5 and the roof. We want to add Levels 1 and 2.
  * Selecting the levels 3-5 and roof, we can change the electrical view template to "none", and discipline to ["coordination"](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Coordination.png).
  * Then, we make duplicate levels 3-5 and roof with detailing, renaming them to the power naming convention (not renaming the level here).
  * Then, we put the view template back to electrical to copy the views to the electrical view tab in the [Project Browser](https://github.com/ashthemech/Revit-Learning/blob/main/Starting%20a%20Revit%20Project/Electrical%20Power%20New%20Views.png).
  * Views are used a lot in Revit, copying, manipulating, and then removing views but want to be organized about it. 

</details>
</details>

<details>
<summary> 3. Revit Electrical </summary>

  Key Takeaways:
  * Learned how to place a standard receptacle on a wall.
  * Learned how to place panels, rename them, and copy them with a different voltage.
  * Learned how to create a panel schedule from existing circuits and explored how to edit a panel template.
  * Learned how to place lighting in a room and check if a recessed fixture is recessed correctly.
  * Learned how to add a switch, duplicate a switch, and connect switches to a lighting fixture.
  * Learned how to create a lighting circuit with the panel, and create a page view for the panel schedules.
  * Learned how to add wires to receptacles and lighting with Revit's automatic placement and manual point to point wiring.
  * Learned how to tag circuits, edit tag parameters and create a new tag from an existing tag.
  * 


<details> 
<summary> Notes </summary>

  **Adding Recepticals**
  * Now we want to add some receptacles into our building.
  * Making sure I was in "Level 1 - Power", we want to add receptacles into the Office Space 101.
  * We go into the "Systems" Tab, then the device pulldown for "Electrical Panel" and select ["Electrical Fixture"](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Electrical%20Fixture%20Tool.png).
  * I ensured I had the "standard" receptacle selected and made sure "place on vertical face" was on.
  * I [placed](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Placed%20Recepticals%20in%20Office%20and%20Reception.png) 3 in the Office 101 Room and also 3 in the Reception 102 room.
    * I also noted that the Loads tab in the properties is grayed out since there is no panel or circuit number specified. 


  **Adding Panels**
  * We have receptacles in our model, but we can't yet circuit them. That's what the panel does.
  * Here I will add a panel, give it a name, and look at the distribution system.
  * In Level 1 - power we can zoom into the Electrical room.
  * Then on the Systems tab in the electrical panel we can click on "Electrical Equipment".
  * We scroll down to select "Lighting and Appliance Panel Board - 208V MLO 225A".
  * I placed it on the [bottom wall](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/PP-1%20Panel%20Placement.png), then selected the panel to access the identity data.
  * I named the panel PP-1, and noted it has a distribution system - to power something with it, these distributions must match.
  * I copied the panel we placed and set the copy to the [right of the original panel](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/LP-1%20Panel%20Placement.png), making it a 480V MLO at 250A and named it "LP-1".


  **Creating a Circuit**
  * Now that we have panels and receptacles placed, we can create a circuit. A circuit is required to populate a panel schedule.
  * In our office, we can select any one of the receptacles and click on "Power" then select PP-1. 
  * Then, clicking on "Edit Circuit" and holding down CTRL, I selected the remaining receptacles in the office.
  * Then I made sure the Load Name was just "OFFICE 101 POWER" [(omitting "Receptacle")](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Office%20101%20Circuit.png).
  * I repeated this process for [RECEPTION 102](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Reception%20102%20Circuit.png).


  **Panel Schedules**
  * Panel schedules are a unique kind of schedule in Revit - you produce it by simply clicking on the panel and clicking "Create".
  * In Level 1 - Power in our electrical room, we select the PP-1 panel.
  * Then, I clicked Create Panel Schedules tab and used the [Default Template](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/PP-1%20Panel%20Schedule.png).
  * If we click on our Office circuit, notice we can move it down, across, up, or "to".
  * We can reindex, we can lock or unlock it, and edit the fonts.
  * If we click on an open circuit, we can assign a spare or a space, or can label placeholders.
  * Now, in the Project Browser, we have a new Panel Schedule drop down available showing our Panel Schedules.
  * In the manage tab, we can manage the panel schedule templates.
  * We can have a Branch panel, Data Panel, or a Switchboard. We can also see the available templates in Revit or change the panel configuration.
  * In the Apply Templates tab we can apply a template to an existing panel schedule.
  * If we click on Edit for the Default Branch Panel Schedule, we can [modify the template](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Edit%20Default%20Branch%20Panel.png) with carrots denoting fields.
  * We can upload a picture, merge and unmerge cells, or change the default fields.
  * Now, any fixtures that are added or removed from that panel will be automatically updated.


  **Adding Lighting Fixtures**
  * Now in 1 - Ceiling Elec, let's add some lighting - first ensure lighting fixtures are visible in the graphic override settings.
  * Again in the Systems tab, we can go to "Lighting Fixtures" and select "Plain Recesses Lighting Fixture - 2x4 - 277".
  * Ensure "Place on Face" is selected, I [placed two lighting fixtures](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Lighting%20in%20Office%20101.png) in the Office 101 room.
  * I repeated the process to [place two in the Reception 102 room](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Lighting%20in%20Office%20and%20Reception.png) as well.
  * Note - make sure if you want to put a fixture in the ceiling, it is indeed IN the ceiling.
    * To do this, we can [cut a section](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Section%20for%20Lighting.png) by going to the view tab and creating a slice with the "Section" button.
    * It will display quite a large section, but we can use the grips to zoom in and [confirm our lighting fixtures](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Section%20View%20for%20Lighting%20Cropped.png) are indeed recessed.
  * Most lighting manufacturers have lighting families that can be used.


  **Adding Switches**
  * We have our lights, but we need to add switches so we can turn them on and off.
  * Back into Systems tab. clicking Device and then Lighting to add a "Door" switch near the doors.
  * Making sure Place on Vertical Face was selected, I [added a switch](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Addding%20a%20Door%20Switch.png) next to the door, then [removed the label](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Removing%20a%20Switch%20Label.png) to clean it up by clicking "Edit Type".
  * I then Left clicked on the switch, hit "Create Similar" and [added another switch](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Duplicating%20a%20Switch.png) to the reception room.
  * Then to circuit it,  we can select [one of the fixtures](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Selecting%20a%20Light.png) in the office, then click "switch -> add switch" and [select the appropriate switch]().
  * Then, "Edit Switch System" to [select the other lighting fixture](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Creating%20a%20Switch%20System.png) aswell, then repeat for the Reception room.
  * If you hover over the switch, and hit "tab", you can [see what it controls](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Using%20Tab%20to%20See%20Controls.png).


  **Creating a Lighting Circuit**
  * Still in the Ceilings Electrical view for the 1st floor, we select a light fixture and click power.
  * Then, making sure LP-1 is the panel we use, we click edit circuit to add the other light fixture, then [changing the name](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Office%20101%20Lighting%20Power.png) to OFFICE 101 LIGHTING.
  * Then, the process can be repeated for the Reception room.
  * Now we create a [panel schedule](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/LP-1%20Panel%20Schedule.png) for the lighting of these two rooms - note you can also edit the names in here.
  * We can add our panel schedules to a [new sheet](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Panel%20Schedule%20Sheet.png), naming it "PANEL SCHEDULES".


  **Creating a Switching Circuit**
  * Now that Revit knows you have a circuit in place, it can automatically draw in the wiring - we will do both ways, the automatic way and adding point by point.
  * In our Power floor plan on Level 1, if we hover over a receptacle and hit tab key once, it will kind of [wire it in](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Adding%20Wires%20to%20Office%20Receptacles.png). 
  * If we then select the fixture, we will get a chamfered wire or an arc wire. Let's select edit path.
  * Here, we can select farthest distance or all devices - let's keep it on farthest device for now.
  * Going back into modifying the wires, we can click on ["Generate Arc Type Wiring"](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Wires%20in%20Office%20with%20Ticks.png).
    * A note on these wires - we can add or subtract tick marks, but some firms do not show them at all.
    * To turn them off, go to systems tab and electrical settings dropdown, then into wires and set show tick marke to never to [get rid of them](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Wires%20in%20%20Office%20Without%20Ticks.png).
  * I repeated the process for the [Reception room](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Wires%20in%20Reception%20Added.png), then went back into the Ceiling Electrical for Level 1.
  * This time, I [manually added](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Wires%20for%20Lighting%20in%20Office%20Manual.png) the wires by going into the wire drop down, selecting arc wire and adding the light wires and the homerun wire.
  * I repeated the automatic process for the Reception room by tabbing until it showed the [homerun wire view](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Wires%20in%20Reception%20-%20Homerun%20Tab.png), then [added the wiring](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Wires%20in%20Reception%20Added.png).


  **Creating and Labeling a Wiring Plan**
  * Now we can use the benefits of "information modeling" - to annotate a plan, we don't necessarily have to type anything in.
    * All of the descriptive tags are going to be parametric. We will annotate our plans using "smart tags".
  * On Level - 1 Power in the Electrical room I clicked Annotate and then Tag by Category - if we hover over the panel, it will auto-tag them.
  * I changed the Leader from "Attached" to "Free", then added a [tag to PP-1](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/PP-1%20Tagged%201.png).
  * Then clicking on the tag, I went to Edit Type to add an arrow, then I moved it [below the electrical room](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/PP-1%20Tagged%203.png).
  * I right clicked on the PP-1 tag to create similar to tag [LP-1 panel](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/LP-1%20Tagged.png).
  * Then back up to the office space, clicking tag by category again to tag the [office circuit](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Office%20Power%20Tagged%203.png).
  * "3" is not very descriptive, so let's edit it by selecting "Edit Family".
  * Clicking on "Edit Label", I added Panel from the Category Parameters into the [Label Parameters](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Adding%20Panel%20to%20Power%20Tags.png).
  * Then clicking "Load into Project" and "Overwrite Existing Version" we now have the [associated panel too](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Office%20Power%20Tagged%20w%20Panel.png).
  * I created similar again to tag the [reception circuit](https://github.com/ashthemech/Revit-Learning/blob/main/Electrical/Reception%20Power%20Tagged.png).


  **Adding Conduit**
  * 


 
  
</details>
</details>
