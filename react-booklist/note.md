#### First Component

```js
function Greeting() {
  return <h2>My First Component</h2>;
}

// arrow function

const Greeting = () => {
  return <h2>My First Component</h2>;
};
```

- starts with Capital letter
- return JSX
- always close tag <Greeting/>

##### Root Component

index.js

```js
import React from "react";
import ReactDOM from "react-dom/client";

function Greeting() {
  return <h2>My First Component</h2>;
}

const root = ReactDOM.createRoot(document.getElementById("root"));

root.render(<Greeting />);
```

#### Local Images (Public Folder)

- save image
- create images folder in public
- replace url in the src - './images/imageName.extension'
- './' because assets are on the same server

```js
const Image = () => <img src="./img/book1_.jpg" alt="American Prometheus" />;
```

- whatever assets we place in public - instantly available
- domain(localhost)/asset

#### Map Mathod

- array mathod
- returns a new array
- does not change the size of original array (unlike filter)
- uses values from original array when making new one
