# Advanced Redux Day One

## Specialization - What to Expect

 - Meet Thursday, Friday, Monday Tuesday 9:00-10:30
 - One or two people will report on a topic
 - Group discussion
 - Prep/reading for next day
 
 ## How to present
 - Each redux club member choses a topic to report out to classmates. This means each presenter will read provided learn.co readme and linked bloged post for their topic, as well as any other blog posts or documentation they find on their own. (Plan to spend a few hours reading and preparing.)
 - When presenting, be sure to explain the topic in broad terms, defining any terminology or concepts encountered, and in specific terms (how it is implemented). The presentations can be informal and interactive. You don't need to be an expert or have everything figured out!
 - The presentation to classmates can include examples from presenter's own project or show code examples from documentation or blogs.
 - As a presenter, discuss questions encountered during research, or problems with implementations, as well as the advantages (and possible disadvantages) of the approach. 
 - If necessary, slack out links or an outline of the presentation to the group. 
 
 ## Topics
  - Thunk Middleware
  - Normalizing Data and Normalizer
  - Selectors
  - Higher Order Components
  
  # Day One To Do
 - Review Redux Flow
 - Combine reduxers review
 - Choose topics
 - Begin preparing topic presentations and reading advanced redux curriculum
 
 # Redux Flow
 
 # Combine Reducers
 ### what is it and why use it
 - Reducers dictate how an application's state will change.
 - **Combine reducers** gives us the ability to **combine reducers** °_o from separate files into one reducer. 
 - use Redux's combine reducers, so that we can keep reducers for different resources separate, and combine them when creating the store. 
 - Why use combine reducers:
    - keep logic for resources separate and organized
    - prevent long switch statement
    - ??
- <a href="http://redux.js.org/docs/api/combineReducers.html#notes">Documentation Notes</a>  
### implementation
- create multiple reducers
- create and index file for the root reducer and import redux's combine reducer, as well as the other reducers.
- call combine reducers, passing in key/value pairs with each reducer as a value. The key can be whatever name you pick, though ideally it should represent the piece of state it's altering. 
- ES6 allows abbreviated syntax: ```combineReducers({ users, snacks }```
- Or, even more abbreviated: 
```
import * as reducers from './reducers'
const todoApp = combineReducers(reducers)
```
  
  **https://learn.co/tracks/react-and-redux/redux-library/multiple-resources-with-redux/combine-reducers-codealong**
  **check the dispatch on new snack**
 
