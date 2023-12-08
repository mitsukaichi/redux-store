# 22 State: Redux Store 

## About this project

This project was done as a homework assignment in UC Berkeley Full Stack Coding Bootcamp. 
The students were given a functioning e-commerce platform and refactor the code to use [Redux](https://redux.js.org/) instead of the Context API.

## Use

- deployed link: https://vast-fortress-80312-70af27ef39cc.herokuapp.com/
- screenshot: ![screenshot](https://github.com/mitsukaichi/redux-store/assets/45612744/8ba3c8d0-616c-47ad-9573-9a83756e9218)

## Things I learnt form this challenge

- Difference between Reducer, Context API and Redux

Throughout the course, I was mixing up Reducer, Context API and Redux, not knowing what functionality belongs to which. After going through this project I have better understanding of what is Reducer, what is Context API and how Redux brings the benefit of Reducer and Context API combined. 

- With Redux, the component inside of `<div className="App">` will only run once when the component is called and doesn't have access to the state which is called by `store.getState()`. You need the `Provider` from `react-redux` at root to provide the `store` to child components, and you need to create a function map the redux state to a react component's props and connect that function to the component using `connect`.
The following stackoverflow answers were really helpful to solve this issue.
- [Redux: Component is not updating after state is updated](https://stackoverflow.com/questions/67827184/redux-component-is-not-updating-after-state-is-updated)
- [React component not updating when store state has changed](https://stackoverflow.com/questions/35917210/react-component-not-updating-when-store-state-has-changed)

## License

MIT License

Copyright (c) [2023] [Minami Mukai]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
