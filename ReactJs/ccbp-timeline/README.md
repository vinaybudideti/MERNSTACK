
Live demo [ccbptimeline.ccbp.tech](https://ccbptimeline.ccbp.tech)

### Refer to the image below:

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/ccbp-timeline-output.gif" alt="ccbp timeline output" style="max-width:70%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

### Design Files

<details>
<summary>Click to view</summary>

- [Extra Small (Size < 576px) and Small (Size >= 576px)](https://assets.ccbp.in/frontend/content/react-js/ccbp-timeline-sm-output-v2.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px)](https://assets.ccbp.in/frontend/content/react-js/ccbp-timeline-lg-output.png)

</details>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>
<summary>Functionality to be added</summary>
<br/>

The app must have the following functionalities

- Initially, the page should display the timeline items list using **Chrono custom rendering** based on the `categoryId`
- The `TimelineView` component is provided with `timelineItemsList`. It consists of a list of timeline item objects with the following properties in each timeline item object

  - The `timelineItemObject` with `categoryId` as `COURSE` will have the following properties

    |     Key     | Data Type |
    | :---------: | :-------: |
    |     id      |  String   |
    | categoryId  |  String   |
    |    title    |  String   |
    | courseTitle |  String   |
    | description |  String   |
    |  duration   |  String   |
    |  tagsList   |   Array   |

  - The `tagsListObject` will have the following properties

    | Key  | Data Type |
    | :--: | :-------: |
    |  id  |  String   |
    | name |  String   |

  - The `timelineItemObject` with `categoryId` as `PROJECT` will have the following properties

    |     Key      | Data Type |
    | :----------: | :-------: |
    |      id      |  String   |
    |  categoryId  |  String   |
    |    title     |  String   |
    | projectTitle |  String   |
    | description  |  String   |
    |   imageUrl   |  String   |
    |   duration   |  String   |
    |  projectUrl  |  String   |

- If the value of the key `categoryId` in `timelineItemObject` is `PROJECT` then Project card should be rendered
  - The `ProjectTimelineCard` should consist of **Visit** link when a user clicks on it, then the page should be navigated to the respective project
  - The `ProjectTimelineCard` should consist of a **Calendar** icon with respective `duration` text
- If the value of the key `categoryId` in `timelineItemObject` is `COURSE` then the Course card should be rendered
  - The `CourseTimelineCard` should consist of a **Clock** icon with respective `duration` text
- Give the timeline items list data as a value to `items` prop for the `Chrono` component from **react-chrono**, so that the title will be displayed beside each card

</details>

<details>
<summary>Components Structure</summary>

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/ccbp-timeline-component-structure-breakdown.png" alt="component structure breakdown" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

</details>

<details>
<summary>Implementation Files</summary>
<br/>

Use these files to complete the implementation:

- `src/components/TimelineView/index.js`
- `src/components/TimelineView/index.css`
- `src/components/CourseTimelineCard/index.js`
- `src/components/CourseTimelineCard/index.css`
- `src/components/ProjectTimelineCard/index.js`
- `src/components/ProjectTimelineCard/index.css`
</details>


