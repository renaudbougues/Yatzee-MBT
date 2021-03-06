Yatzee-MBT
==========

<b>Model-based testing of an implementation of the Yatzee Game Rules using Spec Explorer.</b> <br />
<b>Spec Explorer</b> is a powerful tool allowing the tester to define a <b>model progam</b> with <b>actions</b> and <b>rules</b>.<br\>
"Action" methods represent "mockup" behaviors of the real implementation under test (IUT).<br\>
"Rules" are defined on action methods and mostly indicates the conditions (or program state) under which a call to the action is a valid "move".<br\>
Spec Explorer engine compute the entire model program behaviour by exploring all possible scenario of action's valid combinations.<br\>
In practice, any search tree will be TOO wide. (test scenario for any unrestricted types such as double or string will be impractical).<br\>
The config.cord is a "coordination" file that allows to define <b>model slicing</b> constructs. That is, typically constraint on input ranges and specific scenario paths.<br\>
Spec Explorer output the program's behaviour model after exploration.<br\>
Then <b>code generation</b> of tests is offered from the behaviour model.<br\>
