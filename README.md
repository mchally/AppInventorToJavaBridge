# AppInventorToJavaBridge
This repository is dedicated to modifying the MIT AppInventor source code to include translation of Blockly to JavaBridge.

The main purpose of this translation is to ease the transition for students from a visual blocks language to actually being able to see the JavaBridge code associated with the blocks they dragged and dropped to create their app in AppInventor.

This version does not download a file directly, but when building the apk will generate a file in the Project.aia if you change it's extension to .zip. The file will be called Screen1.yail, but is actually runnable Java code if the JavaBridge library is on the build path and the extension is changed to .java. 

1) export project.aia
2) change .aia to .zip (make sure to press use zip if prompted)
3) decompress, navigate through src/ to Screen1.yail
4) change extension from .yail to .java
5) configure your build path to have JavaBridge and necessary libraries
6) run as normal java program
