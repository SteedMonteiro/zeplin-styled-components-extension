# Zeplin Styled Components - React Native Extension


Generates styled-components snippets from colors, text styles and layers for react-native.

This is an adaptation from the [original styled components extension](https://github.com/dazzz/zeplin-styled-components-extension) to make the subtle changes needed for use in react-native.

Sample component output:
```js
styled.View`
  ${Typography.Button};
  width: 69px;
  height: 16px;
  font-weight: 500;
  color: ${Colors.White};
`
```

Sample colors output:
```js
export default {
  White: '#ffffff',
  Blue300: '#4a90e2',
  Gray300: '#9b9b9b',
  Black300: '#000000'
}
```

Sample text style output:
```js
import { styled } from 'styled-components/native'

export default {
  Body: styled.Text`
    font-family: OpenSans;
    font-size: 18px;
    line-height: 24px;
  `,

  Title: styled.Text`
    font-family: OpenSans;
    font-size: 48px;
    font-weight: bold;
    line-height: 52px;
  `,

  Button: styled.Text`
    font-family: OpenSans;
    font-size: 16px;
    font-weight: 500;
    line-height: 16px;
    letter-spacing: 1px;
  `
}
```

## TODO
- Add parameter for exporting colors with alpha channel using `hexToRgba` function.
- Add parameter for including breakpoints.
