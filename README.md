# Comments App Project

In this project, I have built a **Comments App** by applying the concepts learned so far.

## Output Preview

![Comments App Output](https://assets.ccbp.in/frontend/content/react-js/comments-app-output-v0.gif)

## Design Files

<details>
<summary>Click to view</summary>

- [Extra Small (Size < 576px) and Small (Size >= 576px)](https://assets.ccbp.in/frontend/content/react-js/comments-app-sm-output-v2.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px)](https://assets.ccbp.in/frontend/content/react-js/comments-app-lg-output-v0.png)

</details>

## Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`

</details>

## Functionality Implemented

- Initially, the list of comments is zero, and the input fields are empty.
- When non-empty values are provided and the **Add Comment** button is clicked:
  - A new comment is added to the list of comments.
  - The comments count is incremented by one.
  - The input fields for name and comment are updated to their initial values.
- When the **Like** button of a comment is clicked:
  - If the image for **Like** is ![Like](https://assets.ccbp.in/frontend/react-js/comments-app/like-img.png), then it changes to ![Liked](https://assets.ccbp.in/frontend/react-js/comments-app/liked-img.png).
  - If the image is already ![Liked](https://assets.ccbp.in/frontend/react-js/comments-app/liked-img.png), it changes back to ![Like](https://assets.ccbp.in/frontend/react-js/comments-app/like-img.png).
- When the **Delete** button of a comment is clicked:
  - The comment is deleted from the list of comments.
  - The comments count is decremented by one.

## Components Structure

![Component Breakdown Structure](https://assets.ccbp.in/frontend/content/react-js/comments-app-component-breakdown-structure-v0.png)

## Implementation Files

I have completed the implementation using the following files:

- `src/components/Comments/index.js`
- `src/components/Comments/index.css`
- `src/components/CommentItem/index.js`
- `src/components/CommentItem/index.css`

## Quick Tips

- The `formatDistanceToNow` function from the **date-fns** package is utilized to return the gap between the given date and now in words.

```js
import { formatDistanceToNow } from 'date-fns';

console.log(formatDistanceToNow(new Date())); // less than a minute
