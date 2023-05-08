Download Link: https://assignmentchef.com/product/solved-prog1360-assignment-2-led-toggle-loop
<br>
<h3>Demonstration – Building on Labs</h3>

This assignment builds on the labs so far, and requires that you now write some code.

The Demonstration section of this document outlines the items you are required to show.

<h2>Tasks</h2>

<h3>Changes to the C Code</h3>

Modify the xx_hook.c file from your previous labs as follows:

Change the declaration for

int add_test(int x, int y)

to

int xx_led_demo(int count, int delay)

where xx is replaced by your initials (i.e. if your name is John Smith, it would be js_led_demo).

Change the name of your C function (the one that you add to the menu) to xxA2, where xx corresponds to your initials (i.e. if your name is John Smith, it would be jsA2). Make sure you change the corresponding ADD_CMD macro at the bottom of the file.

Modify the xxA2 function to retrieve two arguments from the user as shown in your lab – count (uint32_t) and delay (uint32_t). Provide sensible defaults if the user does not provide one or both parameters.

Change the user interface text to reflect the fact that we are now doing something other than adding numbers together.

<h3>Changes to the Assembly Code</h3>

Modify the xx_asm.s code from your previous lab as follows:

Change the name of the function add_test to xx_led_demo, corresponding to the change you made to the declaration in the C file. Be sure it has been changed everywhere it needed to be changed.

Remove the old contents of add_test, replacing it with new code that does the following:

<ol>

 <li>Toggles all 8 LEDs using a loop. To make your life easier, they do not need to be in order.</li>

 <li>Delays between LEDs toggling according to the delay passed by the user.</li>

 <li>Repeats this cycle the number of times specified by the user.</li>

</ol>

<h2>Demonstration</h2>

Please note that you must be prepared before offering to demonstrate your code. You must demonstrate the code that you have submitted to the eConestoga dropbox.

For this assignment, you will demonstrate the following items. You may use a lab PC or your own. If needed, you may use a classmate’s VM, but you MUST run your own code and only your own code. You must demonstrate in your regularly scheduled lab period. If you demonstrate modified code, you will receive a late penalty according to how long it has been since the dropbox deadline.

<h2>Requirements</h2>

<ol>

 <li>Your xx_hook.c and xx_asm.s code as taken directly from the drop box compiles.</li>

 <li>Your code deploys with sudo make program.</li>

 <li>Your code runs with no parameters provided (sensible defaults).</li>

 <li>Your code runs with only a count provided (and that count is used correctly).</li>

 <li>Your code runs with both a count and a delay value provided (and those values are used correctly).</li>

</ol>

<h2>Code</h2>

You will paste your code into the eConestoga quiz boxes as requested. It will be evaluated on the following criteria.

<h3>Functionality</h3>

Your program behaves as specified.

<h3>Proper use of Registers, the stack, and link register</h3>

Only necessary items (no more, no less) are pushed onto the stack. Your function calls use the link register appropriately.

Code Readability

Your code is properly indented, does not wrap or have long lines, and can be logically understood.

Code comments

As this is assembly language, you must extensively comment any code that is unclear (i.e. nearly every line).

Document Requirements

You do not need to submit a document for this assignment.

Be sure to complete the eConestoga quiz appropriately.