## What is Redux?
A state management system for cross-component or app-wide state

There are 3 states:
Local State: State that belong to the single component
    Eg: Listening to user input in a input field: toggling a "show more" details field
Cross Component State: State that affects multiple components like open/close of a modal overlay: Requires "prop chains"/"prop drilling"
App Wide State: State affects entire Application (most/all components) Eg: user Authentication status: Requires: "props chains"/ props drilling


The props chains and props drilling can become a bit cumbersome so therefore context can be used 
React Context is the build in feature of the React which helps in managing cross component and application wide state easier


Redux Context: Solves the same problem, used for managin app wide state


Redux: For Cross-component or app-wide state
You can use both mixing and matching is all posible


Context can be cumbersome in some cases.
In more complex apps, managing react context can lead to deeply nested JSX code and or huge context provider components
React Context is not optimized for high- frequeny state changes

Context: COntext is ready to be used for low frequency unlikely updated like locale and theme
The Changes that happen very frequently it is not that great

Performance can be bad if you are managing wrong kind of state with Context.


## How Does Redux work?
Redux is all about having one central data store in your application with data mean state

Whichever Application wide state you have you can use Redux for that

If the data changes then the components get to know the changes
Components never never directly manipute the store data so we have the subscription but donot have the data flow in the other direction

Components dont directly manipulate data in the Store for that we use the concept called reducer

This reducer we setup this reducer functions is used for Mutating or  chaning the store data

Reducer Function take some input and transform that input they reduce it for Example they reduce the list of Numbers
to sum of that number

They take some input and spit our a new response


Actions: COmponent Dispatch the Actions Component trigger certain actions
Action is just simple Javascript Object whcih descripbed the kind of Operation the reducer should perform.

Thereore Redux then forward actions to the Reducer  reads the description of the Desired Operation
and then this operation is performed by the Reducer

Reducer functions should be pure functions Same input leads to same output there should not be any sideeffects

Its the Reducer works together with the store.
















