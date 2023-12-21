---
id: gghyc3faf737q5dk3blqken
title: Callback Hell
desc: ""
updated: 1703154545233
created: 1703146840209
---

- Also, known as **Pyramid of Doom**.
- Callback Hell is essentially nested callbacks stacked below one another forming a pyramid structure. Every callback depends/waits for the previous callback, thereby making a pyramid structure that affects the readability and maintainability of the code.

Example:
![Callback Hell](image-13.png)

- Code is growing horizontally.
- With prmoises, we can flatten the callbacks and seperately define each function.
- Then make a promise chain to chain our asynchronous functions together in a much more readable and maintainable way.

Example:
![Promise chain](image-14.png)

- Another better way, using async-await:

![async-await](image-15.png)
