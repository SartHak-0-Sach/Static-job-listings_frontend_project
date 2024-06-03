# Static Job Listings

## Discover your next career move with the Static Job Listings website. Browse through a curated list of job opportunities and find the perfect fit for your skills and aspirations.

## Table of Contents

- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)
- [Got Feedback for Me?](#got-feedback-for-me)

## Overview

### The Challenge

Discover your next career move with the Static Job Listings website. Browse through a curated list of job opportunities and find the perfect fit for your skills and aspirations.

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![Design Preview](./design/active-states.jpg)

### Links

- Solution URL: [GitHub Repository](https://github.com/SartHak-0-Sach/Static-job-listings_frontend_project)
- Live Site URL: [Live Site](https://job-listing-frontend.netlify.app/)

## My Process

### Built With

- HTML5
- CSS3
- JavaScript

You will find all the required assets in the `/design` folder. The assets are already optimized.

There is also a `style-guide.md` file containing the information you'll need, such as color palette and fonts.

### What I Learned

- Designing an intuitive user interface for job seekers to easily find relevant job listings
- Implementing interactive features for filtering and searching job listings based on various criteria
- Creating a responsive layout for seamless browsing across devices

```js
class JobBoard {
  constructor() {
    this.mainContainer = document.querySelector(".main-container");
    this.dataBox = document.querySelector(".data-box");
    this.dataBoxStored = document.querySelector(".data-stored-box");
    this.clear = document.querySelector(".clear-data");
    this.clear.addEventListener("click", this.clearData.bind(this));
    this.mainContainer.addEventListener("click", this.selectButton.bind(this));
    this.dataBox.addEventListener("click", this.deleteDataStorage.bind(this));
    this.dataStored = [];
    this.newData = null;
    this.fetchData();
  }

  fetchData() {
    fetch("./data.json")
      .then((res) => res.json())
      .then((data) => {
        this.newData = data;
        this.renderData(this.newData);
      })
      .catch((error) => {
        console.error("Error fetching JSON file:", error);
      });
  }
```

### Continued development

The continuously learning journey of a programmer never ends. This project made me realize that there are many concepts that I need to work upon including fundamentals like flex-box and its properties, to more complex concepts like working with fetch and async await in javascript. These areas are some that I think I need to work more upon in the upcoming future as they highlight some of the most significant regions of web development that are important for every developer to know of. 

These key points mentioned here will help me grow accountable and consistent towards improving at writing good quality code and be a successful full stack developer one day.

### Useful resources

- [Harkirat Singh course notes](https://github.com/SartHak-0-Sach/harkirat-singh-course_code_and_notes) - I have added notes of all lectures along with code and lecture insights of all weeks along with bonus lectures to help you all as much as I can.
- [My development code and notes](https://github.com/SartHak-0-Sach/cwh-web-dev-playlist_code_and_notes) - These are my notes that I made while working on my development skills in initial days and did these courses. Make sure to star the repository if you like it.✨💫
- [MDN documentation hover state for CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/:hover) - This is an amazing article which helped me finally understand hover states. I'd recommend it to anyone still learning this concept.

## Author

<b><strong>Sarthak Sachdev</strong></b>
- Website - [Sarthak Sachdev](https://itsmesarthak.netlify.app/)
- LeetCode - [@sarthak_sachdev](https://leetcode.com/u/sarthak_sachdev/)
- Twitter - [@sarthak_sach69](https://www.twitter.com/sarthak_sach69)

## Acknowledgments

I feel like the solutions provided on the website and the continuous doubt solving by industry experts on discord for free is something that is unmatched by anyone else and need to be acknowledged for their efforts in improving me as a developer by suggesting the best practices in your respective tech stack.

## Got feedback for me?

I love receiving feedback! I am always looking to improve my code and take up new innovative ideas to work upon. So if you have anything you'd like to mention, please email 'hi' at saarsaach30[at]gmail[dot]com.

If you liked this project make sure to spread the word and share it with all your friends.

**Happy coding!** ☺️🚀
