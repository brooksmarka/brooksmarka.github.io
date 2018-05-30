---
layout: post
title: Working with React
feature-img: "img/reactjamslanding.png"
---

There are quite a few React projects I'm excited to be currently working on.

## Campsite Finder

Currently I'm working on a React Application which will provide offline campsite data for adventurers looking to camp for free on public lands. The app currently renders a map on the screen and provides a marker for each state on the map. Each marker is pulled from an Express server written with Node.js. Not all data is rendered unless it exists within the range of the maps view. Utilizing Google maps as well as an Express server was a great learning experience for me.

#### 50 Locations rendered on a map:

{:.center}
![Brackets]({{ site.baseurl }}/img/locationsonmap.png)

The next steps are rendering data when the user stops dragging the map. While I don't expect to render enough data on the map to experience performance loss this should help optimize the load time of the map. Once that is complete, live data will be used to render onto the map. I'm excited to share updates on this project as it progresses. If you want to follow along you can view the repo [here](https://github.com/brooksmarka/locations_frontend).

## ReactJams

React Jams is a spotify music clone.

{:.center}
![Brackets]({{ site.baseurl }}/img/reactjamslanding.png)

It allows a user to select from a library of albums and play the music directly on the browser. I utilized React Router to handle the client-side page transitions. This approach provides a great user experience because there is no page load. It is viewed as an instant transition for the user instead of a flicker when the page reloads. Another added benefit of this approach is there are fewer requests when transitioning between pages. Only changed content is rendered instead of the entire page. This results in better performance.

React Router makes this easy by simple providing a path and a component to render.

{:.center}
![Brackets]({{ site.baseurl }}/img/reactrouter.png)

You then use a special `<Link />` component provided by React Router to tell the router to transition between pages. When a user follows one of these links, React Router shows the relevant components and updates the URL in the address bar.

{:.center}
![Brackets]({{ site.baseurl }}/img/linkcomponent.png)

I also started using [Tachyons](http://tachyons.io/) which allows me to perform fast inline styling to my components. I like this approach because it allows me to completely compartmentalize my CSS to each component. Tachyons does have some opinions regarding specific sizing of their fonts which can absolutely help with aesthetics. They do this by incorporating design ratios which are pleasing to the eye. The design process is also much easier to debug because all of the styling is present on one page instead of being hidden in a css file that references a specific class(className) in your JSX. I found it faster to create an appealing design since I wasn't constantly switching to a CSS file for all of the changes I was looking to make to a specific class. I just do all of the styling right there in the component. Tachyons did present some issues for me when I tried to fully customize it with [Sass](https://github.com/tachyons-css/tachyons-sass). The color pallate is a little limited and I wanted some interesting color schemes for the site so I just went the CDN route and manually created my own colors to be used with Tachyons.

So far React Jams is looking good! Styling for the Album and Library pages is all that is left to do. If you want to check out the progress you can check out the repo [here](https://github.com/brooksmarka/reactjams).

## Recap

All in all React has been a positive experience for me. Through the use of React Router and Tachyons I have enjoyed the experience! I'm excited to show off these appliations when they have been completed in the My Work section very soon!
