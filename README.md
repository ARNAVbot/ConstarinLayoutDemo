# ConstarinLayoutDemo
Demo app to show various utilities of Constraint Layout

This repo will basically help in getting familiar with some of the basic and dialy use concepts of Constraint Layout that developers generally use in their day-to-day life.

Following topics will be covered in this repo:
1. Autoconnect tool
2. Constraint Bias
3. Changing elements layout_width and layout_height
4. Pack tool and Infer Consteaints tool
5. Barriers
6. Chains

Let's get started
1. Autoconnect tool
2. what does scale type mean android
 
3. The measure of space between the element and the layout's border is known as the constraint bias.
 
If the element is centered, its constraint bias is 50%, which means the element is halfway between the two borders. If the bias is changed to 30% for horizontal constraints, the element would be placed closer to the left border. If it is changed to 70%, the element would be placed closer to the right border. The same is true of vertical constraints: the bias controls how far the element is from the top and bottom borders.
After adding two opposing horizontal constraints—a left and a right constraint—a horizontal slider appears in the view inspector to adjust the bias of the element along the horizontal axis. If you add two opposing vertical constraints, a vertical slider appears to adjust the vertical bias.
 
4.Change the element's layout width and height
The inner lines within the view inspector let you change the UI element's layout_width and layout_height values relative to constraints. Clicking an inner line cycles through the following options for vertical and horizontal constraints:

Fixed: Specify the width/height of the element.

Match Constraints: Allow the element to occupy all available space to satisfy the constraint. (Note that this is not the same as the match_parent value for width or height, which sets the element to occupy all available space of the parent view. You shouldn't use match_parent for any view in a ConstraintLayout.) In the XML file, the value 0dp appears in the layout_width or layout_height attribute for Match Constraints.

Wrap Content: Expand the element as needed to fit its content.
 
5.By using a baseline constraint, you can vertically align elements that have text, such as a TextView, EditText, or Button, so that the text baselines are aligned. Use baseline constraints to align elements that use different text sizes. Baseline constraints are also useful for aligning the text baselines of elements of different sizes.
Refer doc for the above thing -> https://developer.android.com/codelabs/constraint-layout#7
 
6. to expand an element horizontally and vertically using the Pack  tool, and how to use the Infer Constraints  tool. Both tools are in the toolbar at the top of the Layout Editor.
 
7. The Infer Constraints tool infers, or figures out, the constraints you need to match a rough layout of elements. It works by taking into account the positions and sizes of the elements. Drag elements to the layout in the positions you want them, and use the Infer Constraints tool to automatically create the constraint connections.
 
8. What's the difference between Inference and Autoconnect?
The Infer Constraints tool calculates and sets constraints for all of the elements in a layout, rather than just the selected element. It bases its calculations on inferred relationships between the elements.
The Autoconnect  tool creates constraint connections for a selected element to the element's parent.
9. Refer to this -> https://developer.android.com/codelabs/constraint-layout#8 for above
10. You can quickly resize elements by aspect ratio if at least one of the element's dimensions is set to match constraints. -> https://developer.android.com/codelabs/constraint-layout#9
11.  Use barriers to align elements that dynamically vary in size
Barriers allow you to specify a constraint based on multiple UI elements. You'll want to use barriers any time that multiple elements could dynamically change their size based on user input or language.
 
A constraint to a barrier is just like a constraint to another element. However, users don't see barriers, and barriers don't add a level to the app's view hierarchy, which means they don't affect performance.
Refer to this -> https://developer.android.com/codelabs/constraint-layout#10
 
12. Use chains to position multiple elements
You've already learned how to center a single UI element. In this exercise you will learn how to center multiple elements at once using a chain. A chain is a group of elements that are linked to each other with bi-directional position constraints.
When you create a chain, you can position all of the elements as a group, and center all of your chained elements as if they were a single element. -> https://developer.android.com/codelabs/constraint-layout#11
13. There is also a button in the toolbar which helps to delete all the constraints in 1 go.

