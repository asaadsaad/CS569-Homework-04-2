# CS569 Homework 04
## Angular Change Detection
The application has the following components:  
* AppComponent (root)
  * ChildOneComponent
  * ChildTwoComponent
* The root component has two states: `{ChildOne: 0}` and `{ChildTwo: 0}` and display both counts.
* The root component has two buttons, one to increment `{ChildOne: 0}` immutably and the other to mutate it.
* Add another two buttons to the root component to increment `{ChildTwo: 0}` immutably and to mutate it.
* The ChildOne component will receive the root component state `{ChildOne: 0}` and display it.
* The ChildTwo component will receive the root component state `{ChildTwo: 0}` and display it.
## Create `results.md` file and write down your answer
* Implement `OnChanges` and `DoCheck` interfaces for the children components. 
* Notice when each hook is triggered. Write down your results.
* Optimize the application performance so any child component does not have to be included in the change detection cycle unless their input value has changed. 
* Which buttons would you remove to have the application comply with your optimization? Why?
