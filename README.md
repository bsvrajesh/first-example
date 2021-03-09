# first-example


This is a utility belt for React based  plugins.


## Install

In your UI plugin project:


## API

#### `genericViewFromComponent(reactComponent: React.Component): DNAView`

Adapts a React component to a dna platform generic view.  Takes one argument - a React component .
This allows React components to be used as DNA UI platform contributions.

#### Example

```javascript
import React, {Component} from "react"
import {genericViewFromComponent} from "dna-react-utils"

class MyComponent extends Component {
  render() {
    return <div>Sample component</div>
  }
 }
 
 export default genericViewFromComponent(MyComponent)

```


## Form Toolkit


