Download Link: https://assignmentchef.com/product/solved-computergraphics-assignment-16-scene
<br>
5/5 - (1 vote)

Scene

The goal of the application contained in index.html, is to allow the user to control a robotic hand, allowing to open and close fingers with keys 1 to 5:

In file Scene.js there is a procedure DrawSceneTree(S)which receives as parameters an encoding of the scene graph. In particular, S is an array of eight component tuples, each one representing the positioning of one object. Element in position 0 (the first element of the array) is the root node. The components of the tuples represents respectively:

<ul>

 <li>The first three elements (indices 0, 1, and 2) are the x, y and z coordinates of the object, used to define the translation of the object.</li>

 <li>The next three elements (indices 3, 4, and 5) are the rotations around the x, y and z axes, and are used to define the rotation of the object. Euler angles are used in the zxy order.</li>

 <li>The seventh element (index 6) is the index of the first child of the considered node, and the eight element (index 7) is the index of the last child. If the considered element is a leaf of the tree (i.e. it does not have any children), both elements are set to -1.The hierarchy used by the hand is the following:11 12 13 14// 678912340 10 5</li>

</ul>

And the initial definition is shown below:

When the user presses keys, rotations of the parts of the fingers changes. For example, the following figure shows the changes caused by pressing keys 2 to 5, to obtain the pointing finger shown in the figure: