# styled-default
A carefully crafted browser defaults for styled-components.


## Installation
npm:
```
npm install --save-dev styled-default
```

Yarn:
```
yarn add --dev styled-default
```


## Usage with styled-components

```js
// global-style.js
import { createGlobalStyle } from 'styled-components';
import reset from 'styled-default';

const GlobalStyle = createGlobalStyle`
  ${reset}
  /* other styles */
`

export default GlobalStyle;

// app.js
import GlobalStyle from './global-style';

const App = () => (
  <>
    <GlobalStyle />
    <div>Hi!</div>
  </>
}

export default App;
```


You can also use named imports:

```js
// ES Modules
import { reset } from 'styled-default';

// CommonJS
const { reset } = require('styled-default');
```


## License
[MIT](./LICENSE.md)