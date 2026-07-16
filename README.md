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
  * Now we would like to [align the structural Level 2 with the Architectural Level 2]().
  * On Modify Tab, click "Align" - then click the level you want to align TO first, then the level to [bring into alignment]().
  * For the rest of the levels, we can "copy monitor" the rest of them on the collaborate tab.
  * Using select link, [selecting the architectural], then Copy/Monitor, Copy, Copy multiple and CTRL selecting Level 4, 5, and Roof, then hitting "finish".
  * Back to the 1 - Lighting to repeat the process with the [structural model]() with the gridlines. 


  **Creating Floor Plans**
  * 



  
</details>
</details>
