# CP8
11/8/2021
***Java Graphics

Drawing pixel
_Graphics is an abstract class for drawing (think about pencil or crayon)
_Device-independent graphics interface
_JVM creates a Graphics object on a native platform
_Graphics object works with paintComponent to display drawings

Control how a panel is rendered
_Extend the component
_Override
	Protected void paintComponent(Graphics g)

Drawing in the right spot
*Remember to manage your coordinates
_Where is 0,0?
_How “tall” is the screen?
_How “wide” is the screen?
_Which way is positive x? Posotive y?
_Are the coordinates relative or absolute?

Drawing shapes
Graphics class provides many useful drawing utilities
_Drawing icons
…
	
Graphics Words/Strings
_drawString draws the string
_Font class: can select the font
_FontMetrics class: managing fonts
+Can measure the extent of a String before it is displayed
+Use to center text automatically

11/10/21
Beginning GUI programing: 
More Adventurous in Inheritance and Aggregation (and packages)

Packages
_Packages are used to group classes together into meaningful units
_Examples: java.util, java.io
_Very simple to create a package
+When create a new class, enter the package name in the dialog box

Package naming conventions
_Top level domain of organization first
+Subdomains in reverse package order
+Then name the package
_Done to preserve uniqueness of package names
_Examples: edu.ou.game

Access modification and packages
_Protected data is shared when classes share a package
_If you do not give methods and data an access modifier (public, protected, private) it will have package level access

Basic elements of GUIs
_Components (sometimes called widgets): Buttons, Checkboxes, etc.
_Containers collect Components together into a single unit
_Layouts managers
+Determine how the components are organized on a display
+If necessary you can position components without using a layout manager. Generally, this solution is used to specify absolute sizes and positions for components

Two kinds if components
_Abstract Window ToolKit (java.awt)
+Design to use components from platform (OS/XINDOW MANAGER)
+Good idea, but was problematic
 	Have to allow options for all platform options
	 Resulted in heavyweight components
_Swing (javax.swing)
+Components start with J(e.g.JButton)
Container and Component…
_Container inherits from Component
+Container is-a Component
_Container also aggregates Component

Addiotnal Components
_JLabel – labels on the screen
_Fields for users to enter text
+JTextField: single line
+JTextArea

Graphical user interfaces
_At the top level, our GUI should 
_Present information to the user
_Giver the user a means for communicating with the program
_Respond appropriately to these user inputs

Layout managers
_Determine how a set of components within a container are assigned to the screen
_Each container has its own Layout Manager
_Must attach this Layout Manager before components are added
_Useful managers: GridLayout, FlowLayout, BorderLayout, GridBagLayout
