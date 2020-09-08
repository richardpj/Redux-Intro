> All content contained in this talk can be found in the [React Docs](https://reactjs.org/docs/getting-started.html). For specific info on hooks check out the [intro video](https://youtu.be/dpw9EHDh2bM) and the [hooks docs](https://reactjs.org/docs/hooks-intro.html)

# 1. A Short History of React Component Patterns

When react was first introduced in 2013 it included it's own class system for the creation of components via the ```React.createClass()``` method. This method takes a plain old Javascript object and creates a component class. Something like the following:

``` javascript
import React from 'react';

class Contacts extends React.Component {
  constructor(props) {
    super(props);
  }
  handleClick() {
    console.log(this); // React Component instance
  }
  render() {
    return (
      <div></div>
    );
  }
}

export default Contacts;
```

## Test Gist

{% gist d2d9d7d6aff665ab4df0c18e32dc0520 index.html %}

<code data-gist-id="d2d9d7d6aff665ab4df0c18e32dc0520" data-gist-file="index.html" data-gist-highlight-line="1,3,5"></code>

## Test Codepen

<iframe height="265" style="width: 100%;" scrolling="no" title="Codepen Test" src="https://codepen.io/richardpj-the-animator/embed/gOroqew?height=265&theme-id=light&default-tab=html,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/richardpj-the-animator/pen/gOroqew'>Codepen Test</a> by Richard Pierce-Jones
  (<a href='https://codepen.io/richardpj-the-animator'>@richardpj-the-animator</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>
