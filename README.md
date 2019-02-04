# NGRX
NGRX concepts + special focus on effects testing
## What is it? 
Redux version for Angular/rxjs aka store/state management in Angular. I like to say its client-side database.
## Why I use it in my application?
1.	Is my app passing data from one component to another? (Aren’t you breaking a solid principle?)
2.	Is more than 1 component accessing and changing the same data and these changes should be reflected in another components as well?
## How it works? my version
NGRX = Actions + Effects+ Reducer + Selectors
### Flow chart
Check the image in repo
 
### Explanation
1.	Components trigger action.
2.	Effects listen to this action and calls service
3.	Services return data to effects
4.	Effects triggers success action and asks reducer to update state.
5.	Reducer updates store with data. 
 
Yeyyy!!! Data on client-side db
 
How does component get data from db? - 6. Components calls selectors and gets data from store


## References: Special Thanks to below articles
https://blog.angular-university.io/angular-2-redux-ngrx-rxjs/


