# React and Forms

![rr](https://th.bing.com/th/id/R.ec860a78ec07a2d743dfa6097944ff6f?rik=%2fzTe6NpgBoHrZA&pid=ImgRaw&r=0)

## Forms

HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.

## Controlled Components

In HTML, form elements such as input, textarea>, and select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

[MORE](https://reactjs.org/docs/forms.html)
