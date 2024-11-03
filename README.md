# DJS03 Project Brief: Book Connect - Abstractions

#### Discussion and Reflection

After completing the tasks, prepare a brief presentation for your coaching group on the following:
- The rationale behind the refactoring decisions made, including the choice of objects and functions.
The original code was a bit messy with repeated tasks, scattered event listeners, and functions that were doing multiple things at once. This made it harder to read, understand, and change.
To help manage this I used the BookConnectApp as a single object to enscapsulate all the methods and state variables.
For object and functions, key tasks were identified and put them into separate functions like createbookPreview to allow us not to rewrite this each time, and filterbooks to allows filtering based on uer input.

- How abstraction has made the code more maintainable and extendable.
Abstractions makes the app easier to maintain and extend, meaning we can add new features without rewriting everything.

- Any challenges faced during the refactoring process and how they were overcome.
1. Too many global variables make it easy to change values in unlikely places.
For these, it was better to put all important data inside the BookConnectApp object. This help to keep things orgainsed and reduces unexpected changes.
2. The orginal code had separate event listeners all over throughtout hence it was hard to know what each part of the app was listening for.
For these, I grouped all event listeners in a single setupEventListeners function to make it easier to see which events are being handled.

- Reflections on how this exercise has deepened your understanding of JavaScript programming concepts.
1. I spent some time identifying patterns and repetitive code. This planning step helped me see where I could use functions and objects to avoid repeating myself.
2. Abstraction seemed complex at first, but I see now it just means focusing on essentials and hiding details. By using objects and functions to organise tasks.
3. Breaking down tasks into small makes code easier to read and debug.


