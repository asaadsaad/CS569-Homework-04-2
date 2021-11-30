# CS569 Homework 04
## Angular Change Detection
The application has the following components:  
* AppComponent (root)
  * ChildOneComponent
  * ChildTwoComponent
    * ChildThreeComponent (child to `ChildTwo`)
* The root component has two states: `{ChildOne: 0}` and `{ChildTwo: 0}` and display both counts.
* The root component has two buttons, one to increment `{ChildOne: 0}` immutably and the other to mutate it.
* Add another two buttons to the root component to increment `{ChildTwo: 0}` immutably and to mutate it.
* The ChildOne component will receive the root component state `{ChildOne: 0}` and display it.
* The ChildTwo component will receive the root component state `{ChildTwo: 0}` and display it.
## Create `results.md` file and write down your answer
* Implement all component lifecycle-hooks in the root component and write down:
  * Which component lifecycle-hook triggers when the application loads?
  * Which component lifecycle-hook triggers during the change detection cycle?
* Implement `OnChanges` and `DoCheck` interfaces for all the children components in the previous application. 
* Notice when each hook is triggered. Write down your results.
* Optimize the application performance in `ChildOne` and `ChildTwo` component sothey do not have to be included in the change detection cycle unless their input value has changed. 
* Write down which component life-cycle hooks trigger for the `ChildOne` and `ChildTwo` and `ChildThree` components when the buttons are clicked and how it affects the rendering process.
