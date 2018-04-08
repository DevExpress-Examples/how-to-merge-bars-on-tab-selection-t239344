# How to merge bars on tab selection


This example shows how to merge the MainMenuControls on selecting tabs in the TabControl.<br /><br />The TabControl in the example has two tabs, each containing a MainMenuControl. The MergingProperties.ElementMergingBehavior property is used to enable the merging of these MainMenuControls to the root MainMenuControl (located outside the TabControl) on tab selection. Note that the MergingProperties.ElementMergingBehavior property is bound to the TabItem.IsSelected Boolean property. The MergingProperties.ElementMergingBehavior property supports automatic conversion from Boolean values to corresponding ElementMergingBehavior enumeration values.<br /><br />Note:<br />Merging is only supported from a child name scope to the parent name scope. In this example, the root MainMenuControl belongs to the topmost name scope (inherited from the Window object). Child MainMenuControls are located in the tabs that have the ElementMergingBehavior property set. This property implicitly creates a name scope for each tab. This name scope is propagated to the tabs' child elements.

<br/>


