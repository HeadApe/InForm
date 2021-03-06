# InForm
A GUI engine and WYSIWYG interface designer for QB64

Wiki: https://github.com/FellippeHeitor/InForm/wiki

## Event-driven QB64 programs
InForm's main goal is to generate event-driven QB64 applications. This means that you design a graphical user interface with interactive controls and then write the code to respond to such controls once they are manipulated.

## Workflow
After your form looks the way you want it to, click File -> Save to export its contents and generate a .bas source file. Three files are output:
* **.frmbin**
the binary form that can be later edited.
 
* **.frm**
a representation of the generated form in QB64 code. This can be edited in QB64 or any text editor later, if you want to adjust fine details.
 
* **.bas**
the actual program you will add your code to.

### You add code to respond to events:
* *Click*
* *MouseEnter/MouseLeave* (hover)
* *FocusIn/FocusOut*
* *MouseDown/MouseUp* (events preceding a Click)
* *KeyPress*
* *TextChanged* (for text box controls)
* *ValueChanged* (for track bars, lists and dropdown lists)

### There are also events that occur in specific moments, to which you can respond/add code:
* *BeforeInit*, triggered just before the form is shown.
* *OnLoad*, triggered right after the form is first shown.
* *BeforeUpdateDisplay*, triggered everytime the form is about to be repainted.
* *BeforeUnload*, triggered when the user tries to close the program, either via clicking the window's X button, right click in the task bar -> Close or with Alt+F4 (Windows only).
