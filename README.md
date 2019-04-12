
## <a name="section-dwcarousel"> DWcarousel 
### Description

A carrosel container component.

### Props

| Name     | Type   | Required | Default value | Description                                                                                                                  |
| -------- | ------ | -------- | ------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| DWcarousel.Page      | `React.Node`  | `true`  | -         | A component that will be rendered the pages `DWcarousel`|
| children              | `React.Node`  | `false` | `null`    | A component that will be rendered inside the `DWcarousel.Page`. |
| initialPage           | `Integer`     | `false` | 0         | Set a initial page |
| hideIndicators        | `Boolean`     | `false` | `false`   | Set to true to hide the indicators |
| indicatorColor        | `String`      | `false` | `#FFFFFF` | Active indicator color |
| indicatorSize         | `Float`       | `false` | 30        | Indicator bullet size |
| indicatorSpace        | `Float`       | `false` | 15        | Space between each indicator |
| inactiveIndicatorColor| `String`      | `false` | `#DDDDDD` | Inactive indicator color |
| indicatorAtBottom     | `Boolean`     | `false` | `true`    | Set to false to show the indicators at the top |
| indicatorOffset       | `Float`       | `false` | 0         | Indicator relative position from top or bottom |
| inactiveIndicatorText | `String`      | `false` | '•'       | Inactive indicator content ( You can customize to use any Unicode character ) |
| indicatorText         | `String`      | `false` | '•'       | Active indicator content ( You can customize to use any Unicode character ) |
| animate               | `Boolean`     | `false` | `false`   | Enable carousel autoplay |
| delay                 | `Integer`     | `false` | 1000      | Set Animation delay between slides |
| loop                  | `Boolean`     | `false` | `false`   | Allow infinite looped animation. Depends on Prop {...animate} set to true. |
| containerStyle        | `TStyle`      | `false` | {}        | Style container - component `BBCarrosel` |
| pageStyle             | `TStyle`      | `false` | {}        | Style container - component `DWcarousel.Page` |


### Usage example

```javascript
  ...

  render() {
    ...
    return (
      <DWcarousel
        indicatorColor="red"
      >
        <DWcarousel.Page>
          <View>
            <Text>Content 1 - Page 1</Text>
          </View>
          <View>
            <Text>Content 2 - Page 1</Text>
          </View>
        </DWcarousel.Page>
        <DWcarousel.Page>
          <View>
            <Text>Content 1 - Page 2</Text>
          </View>
          <View>
            <Text>Content 2 - Page 2</Text>
          </View>
        </DWcarousel.Page>
      </DWcarousel>
    )
  ...
```