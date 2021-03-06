# About this repository

This is a project I've done as an undergrad to code a Software Product Line based on a notepad for Dr. Eduardo Almeida, the chair
on SPLC Conference in Brazil. There is not much to find here, other than feel nostalgic about my first independent research project :-) 

# Other details

Feature checklist

- Mandatory Feature MenuBar (pre-coded by code author)
- Optional About
- Mandatory Feature TextRaw
- Mandatory Input (Has been inserted into code as an optional variable to identify difficulties)
- Optional SaveAs (requires Input as it uses InputActions class, consequently this feature has no Action class)
- Optional Warn unsaved files (Refer to github commits or to rationale to see how to implement this feature, sligh different way)
- Optional Toolbar Feature (Refer to the Toolbar commit or rationale to see how other features are added to the toolbar).
- Optional Print Feature (Encapsulated the same way as Input Feature)
- Optional Feature Wrap
- Optional Feature Font
    Obs: Currently Font is encapsulated on Wrap feature, will modify that later.

- Optional Feature Find
- Optional Feature Find Next
    Obs: How to use: feature instation with parameters like UndoRedo Feature, refer to FindFeature class inside FindFeature package on its constructors to see available options. Manual will be available later.

- Optional Feature Undo
- Optional Feature Redo
    Obs: Undo and Redo Feature are packed on the same folder, see Rationale to find out why.
        How to use: feature instantiation with parameters (Notepad) {Undo MenuBar} ; (Notepad,true) {UndoMenuBar + UndoToolbar} ; (Notepad,true,true) {UndoMenuBar + UndoToolbar + RedoMenuBar} ; (Notepad,true,true,true) {UndoMenuBar + UndoToolBar+RedoMenuBar+RedoToolBar}
            Other combinations can easily be added to the code by just creating an overloaded constructor on UndoRedoFeature class.
    

Obs: Output features has turned into Mandatory so application can warn users that text on TextRaw feature has not been saved.
A different version without this 'extra warn feature' can be seen on the author Ian version.

- Optional Feature Cut
- Optional Feature Copy
- Optional Feature Paste (has been turned into Optional, see rationale too find out why)
- Optional Feature SelectAll
    How to use: Instantiate like Input file, may use aditional parameter (Notepad,true) for Cut,Copy,Paste to be added to ToolBar as well. SelectAll has no toolbar icon and thus does not have on this version as well.

- Optional Feature Center (has some issue, depending on the screen it appears somewhere else than standard but it is definely not the center :-) (Used original code)
    How to use: Just instantiate like Input file. 
