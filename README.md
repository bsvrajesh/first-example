# first-example


This is a utility belt for React based  plugins.


## Install

In your UI plugin project:
* `npm config set @cisco-dna:registry "https://maglev-nexus.cisco.com:8443/repository/maglev-npm-group/"`
* `yarn add @cisco-dna/dna-react-utils` or ` npm install @cisco-dna/dna-react-utils`


## API

#### `genericViewFromComponent(reactComponent: React.Component): DNAView`

Adapts a React component to a dna platform generic view.  Takes one argument - a React component, and returns a [generic view wrapper](http://dna-ui.cisco.com:8000/guides/contributionmodel/contribution-model/#generic-view-interface).
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


