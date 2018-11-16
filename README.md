# debounce-input-reat &middot; [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/akashishu777/debounce-input-react/blob/master/LICENSE) [![Build Status](https://travis-ci.com/akashishu777/debounce-input-react.svg?branch=master)](https://travis-ci.com/akashishu777/debounce-input-react) [![npm version](https://img.shields.io/badge/npm-v1.1.0-blue.svg)](https://www.npmjs.com/package/debounce-input-react)



## Installation

### NPM

```sh
npm install debounce-input-react --save
```


## Usage
```js
import React from 'react';
import ReactDOM from 'react-dom';
import {DebounceInput} from 'debounce-input-react';

class App extends React.Component {
  state = {
    value: ''
  };

  render() {
    return (
      <div>
        <DebounceInput
          minLength={2}
          debounceTimeout={300}
          onInput={event => this.setState({value: event.target.value})} />

        <p>Result: {this.state.value}</p>
      </div>
    );
  }
}

const appRoot = document.createElement('div');
document.body.appendChild(appRoot);
ReactDOM.render(<App />, appRoot);
```










### License

debouce-input-react is [MIT licensed](./LICENSE).