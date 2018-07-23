# Techdegree-project-4

Before you start
To prepare for this project you'll need to make sure you complete and understand these steps.

 5 steps
Download the project files. Inside you will find an images folder, some mockups, an index.html file, and a no-classes.html file. Don�t modify these files in any way.
Find a css reset like normalize.css to use in the base folder of your project. Searching on google for "normalize css file" should present you with several options to choose from.
Open mobile480px_mockup.png and desktop1400px_mockup.png files. These are your mockup images for what the site should look like at the end of the 480px and 1400px screen widths, respectively. Your goal is to create styles in your sass project using the classes provided in the index.html to make your project match the two mockups provided. Remember, you want to use a mobile first design approach, so style the mobile layout first, and use only min-width media queries.
Open index.html. The structure and classes you need to style the site to the mockups are already in place for you here. We�ve included a comment at the top of the body with a list of the classes we want you to write rules for. You�ll be responsible for creating the sass project that contains all the classes used in this index.html file. No id selectors should appear in the sass project or resulting css, and the only elements you should select directly are p tags, ul tags, and the universal selector.
Open no_classes.html. You should be able to check that you�ve only used the proper classes to style the page by pointing this HTML file to the same css file as index.html. This page should stay completely unstyled when linked to styles.css, matching the no_classes_mockup.png mockup, except for styles applied to the p and ul tags, as well as the universal selector.
Project Instructions
To complete this project, follow the instructions below. If you get stuck, ask a question in the community.

 9 steps
Organize your Sass files.
Create a scss folder in your project.
In the scss folder, create the following subfolders to organize your CSS code into SCSS partial files:
utilities (a folder to contain partials for global variables, extends, mixins, and functions)
base (for the normalize.css file and base styles that are used in the project)
components (to contain partials for each part of your site: grid, typography, navigation, images, buttons, forms)
Each subfolder you create should contain an _index.scss file. You�ll use that file to import each sass partial file in the folder.
Create a css folder for your compiled CSS. As you work on the project, you�ll be able to run sass --watch scss:css from the command line to compile the sass that you write.
Create a styles.scss file in the root of your Sass project (in your �scss� folder).
Import all of your _index.scss partials into this main styles.scss file.
Make sure your imports are listed in the correct order for styling.
Create a partial for variables in your utilities folder
Use this partial to create variables for your repeated values.
At minimum, create variables for fonts, breakpoints, and colors.
Import this partial into your utilities/index.scss file
Create a partial for your mixins in your utilities folder
Inside your mixins partial, you�ll want to create mixins for:

Media Queries
Flexbox settings
Create a partial for your placeholders in your utilities folder
In your placeholder partial, create placeholders for at least the following:

Links
Images
Headlines
Nav items
Components
All your styles for this project will be applied using the classes listed in the comment at the top of the index.html file. You�ll style these classes in the components folder. Try not to combine selectors from two different categories. For example, avoid using .grid__col--8 .link to style the link in the typography section, as it makes the style of links dependent on what grid column they�re in. The best way to organize this is to make a file in the components folder for each of the following:

Grid (recommend using flexbox)
Typography
Navigation
Images
Buttons
Forms
Base folder
In your base folder, include a normalize.css file and create a base.scss file. In the base.scss file, you can only apply styles to three different elements directly:

the universal selector (*)
ul elements
p elements
Check your work
Open the no_classes.html file. If you�ve only used the proper classes to style your page, this page should match the no_classes_mockup.png mockup, and should be almost completely unstyled. If you�ve used element or id level selectors somehow, you�ll see the difference between these two files. Be sure to check that your classes do only what they�re meant to and that each component category doesn�t depend on styles from another category (E.g. - avoid selecting .grid__col--8 .link to style a link in a grid column.) Making these classes as independent as possible will increase the usefulness of using this style guide on other projects.

If you're having trouble with this project, make sure you take a look at this great study guide:
Project 4 Study Guide

Extra Credit
To get an "exceeds" rating, you can expand on the project in the following ways:

 2 steps
Use the flexbox mixin you built to apply flexbox properties in your project.
Use the media query mixin to apply all your media queries.
NOTE:

To get an "Exceeds Expectations" grade for this project, you'll need to complete each of the items in this section. See the rubric in the "How You'll Be Graded" tab above for details on how you'll be graded.
If you�re shooting for the "Exceeds Expectations" grade, it is recommended that you mention so in your submission notes.
Passing grades are final. If you try for the "Exceeds Expectations" grade, but miss an item and receive a �Meets Expectations� grade, you won�t get a second chance. Exceptions can be made for items that have been misgraded in review.
