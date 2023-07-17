# JavaScript Todo List     

This self challenge was encouraged by this [YouTube video](https://www.youtube.com/watch?v=2FeymQoKvrk), see [What I Learned](#what-i-learned)

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)


## Overview

### Screenshot

![desktop screens](/screenshots/desktop.png)
![mobile screens](/screenshots/mobile.png)

### Links

- Live Site URL: [view site here](https://smarko-web.github.io/todo_js/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- js browser memory

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own 
knowledge.

To see how you can add code snippets, see below:

```css
  input[type="checkbox"] {
      appearance: none;
      margin: 0;
      background-color: transparent;
      width: 1.5rem;
      height: 1.5rem;
      max-width: 25px;
      border: 1px solid var(--color-text);
      border-radius: 100%;
      display: grid;
      place-content: center;
      transition: var(--global-transition);
  }
  input[type="checkbox"]::before {
      content: url("https://api.iconify.design/ic:outline-check.svg");
      transform: scale(0);
      transition: var(--global-transition);
  }

  input[type="checkbox"]:checked {
      background-color: var(--color-text-disabled);
      border-color: var(--color-text-disabled);
  }
  input[type="checkbox"]:checked::before {
      transform: scale(1);
      stroke: var(--color-body);
  }
```
```js
  if (localStorage.getItem('tasks')) {
      tasks.map((task) => {
          createTask(task);
      })
  } 

  const completedTasksArray = tasks.filter(task => task.isCompleted === true);
  tasks = tasks.filter((task) => task.id !== parseInt(taskId))

```

in this project I learned how the browser's memory system work, in addition I reinforced some of my array methods skills including ```filter``` and ```map```. With regard to the styling, I got the understanding of how to change the default look of the check box. 

### Continued development

￼I would like to become more proficient in my HTML, CSS, and JavaScript skills before I start doing more advanced web development. As I am practicing these skills, applying the prior knowledge that I have grained from YouTube and other Self paced courses, increasing confidence in web design/development.