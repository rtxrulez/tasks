| Deadline         |
|------------------|
| 23:59 20.02.2020 |

# YouTube client app

[Figma mockup](https://www.figma.com/file/tS3Zqk138yXUmRxSWKDv4r/YouTube-client?node-id=0%3A1)

## Angular. Components. Directives & Pipes task

### Task requirements
The main goal of this task is to implement the main page of the YouTube client app.
You're to enrich previously generated components with necessary functionality and markup.

You can use any UI frameworks/libraries to simplify (facilitate) the creation of your markup. It's recommended to use Angular Material as it’s fully integrated with Angular.

**[YouTube client. Main page JPG](https://github.com/rolling-scopes-school/tasks/blob/master/tasks/angular/main.jpg)**

#### Components structure
- Header
    - Logo
    - Search input with submit button
    - Settings button
    - Login information block
- Filtering criteria block
    - Buttons that represent each sort criterion
    - Input that is related to the "by word or sentence" criterion which is used for filtering results
- Search results block
    - Search result item
        - Video thumbnail
        - Views count
        - Likes count
        - Dislikes count
        - Comments count
        - Video title
        - "More button"

#### Functional requirements
- Once a user is entered the app, The **Header** component should be only shown.
For now, you can enter whatever value which won't influence your search result.
Please note that the **Sorting criteria block** should be hidden
- By submitting the search form, the **Search results block** appears.
- Using the *[response example](https://github.com/rolling-scopes-school/tasks/blob/master/tasks/angular/main.jpg)*, render cards with predefined data
    - The bottom border represents the publication date. Use directive to achieve the result
        - If a publication date is less than month, set border background to green
        - If a publication date is less than 7 days, set border background to blue
        - If a publication date is more that 6 months, set border background to red
- By clicking on the **Settings button**, should toggle the **Filtering criteria block**
    - It should be possible to sort search results by date or count of views
    - Using a pipe, filter search results by value a user types in the input

#### Evaluation criteria
Maximum points - **100**

- [ ] Main layout is implemented (**+10**)
- [ ] Implemented a fake search functionality: by submitting the form on the **Header** component, search results are shown (**+20**)
- [ ] The **Search result item** component contains all the necessary data (**+10**)
- [ ] The **Filtering criteria block** toggle functionality is implemented (**+5**)
- [ ] The colorful cover under the **Search result item** is implemented (**+15**)
- [ ] Search result sorting is implemented (**+20**)
- [ ] Search result filtering by key words is implemented (**+20**)

Fines
- [ ] Failure to submit on time may lead to points loose according to the [Stage #2 requirements](https://docs.rs.school/#/stage2?id=%d0%94%d0%b5%d0%b4%d0%bb%d0%b0%d0%b9%d0%bd%d1%8b)
- [ ] The app has wrong components structure (**-20**)
- [ ] The app doesn't work or has console errors (**-20**)

### Useful links
