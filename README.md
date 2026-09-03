# label-caffeine
a VBA framework that can be added into projects to provide modern day button functionality using labels and the core code.


# Features
* Easy Mouse Hover Events: Removes the need to write out separate mouse up, mouse down events.
* Glass Triggers: Provides mouse hover events to unsupported controls like spins and scrolls.
* Linked Controls: Hover events for multiple controls simultaneously for something like a custom checkbox with 2 or more controls.
* Visual Styling: Create the style on a separate control and reference it. No need to type out RGB colors or other properties.
* Better Control Feedback: Push away buttons, font color changes, Even old school special effect updates all easily customizable for click events.
* Ability to Toggle Tooltips On and Off: Provides a way to disable ControlTipText that would overlap UI with a simple toggle button.
* Minimal User Code Required: All contained in a class and a module, users can make minimal code updates in order to give their userform a modern day feel.


# Concept Workflow (Under Construction):
* Verify prefix
* Check for tag formatting
* check for duplicate keys of useBack = 1 and useBack = 0 in same tag
* check for incompatible properties per type
* store control name, type, tag, clean tag and errors in array of collection
* check for unknown keys
* Check that all groups have at least 2 members
* check that stylefroms exist on form / in collection
* create a simple key exists in collection function
* clean tag by fixing prefix to ; then split all by ;


Explanation
LabelCaffeine: = The identifier
action = The sub that will run when the control is clicked
useBack = true or false with 1 or 0. If 1 then background color comes from styleFrom on hover
useOutline = same as useBack but border color
useFore = same as useBack but fore color (font color)
useFont = same as useBack but full font style with bold, family italic etc.
useImage = same as useBack but image pointer of the styleFrom control image
useSpecial = same as useBack but the specialEffect
styleFrom = The control on the userform that has the properties to use when hovering a control. User can have as many styleFrom controls as they want.
Tooltip = A way to store controltiptext so the user does not always have a tooltip appearing. It can be enabled and disabled with a button on their form that will call labCafTooltipsOn or labCafTooltipsOff
