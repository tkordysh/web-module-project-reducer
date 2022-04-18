# Understanding Questions:
1. What are the steps of execution from the pressing of the 1 button to the rendering of our updated value? List what part of the code excutes for each step.
* The user presses the 1 button.
* 
    - User presses 1 
    - event handler connected to button's onClick method fires (  onClick={() =>  )
    - dispatch method dispatches action 'addOne' to our reducer (   dispatch(addOne())  )
    - addOne returns {type:ADD_ONE} which once fed into reducer as the action.type triggers first case in the switch statement ---case(ADD_ONE)---- and returns :
            return({
                ...state,
                total: state.total + 1
            });
    adding 1 to our current total.
...

* TotalDisplay shows the total plus 1.
