## react-native-slidable-micro-calendar-view

Tested with react-native 0.55

## Add it to your project

1. Run `npm install react-native-slidable-micro-calendar-view --save`
2. `var ScrollableCalendarView = require('react-native-slidable-micro-calendar-view');`



## Demo
<a href="https://github.com/derskeal/react-native-slidable-micro-calendar-view/blob/master/demo.gif"><img src="https://github.com/derskeal/react-native-slidable-micro-calendar-view/blob/master/demo.gif" width="350"></a>

## Basic usage

```javascript
import SlidingCalendarView from 'react-native-slidable-micro-calendar-view';

class SlidingCalendarViewExample extends React.Component {

  constructor(props) {
    super(props);
    this.state = {
      selectedDay: new Date(),
    }
  }

  render() {
    return <View style={styles.container}>
      <SlidingCalendarView
        selectedDay={this.state.selectedDay}
        onDaySelected={this.onDaySelected.bind(this)}
      >
        <View style={styles.content}>
          <Text>Past here your content</Text>
        </View>
      </SlidingCalendarView>
    </View>
  }

  onDaySelected(day) {
    this.setState({selectedDay: day});
  }
}
```

## Example

See
[examples/SlidingCalendarViewExample](https://github.com/derskeal/react-native-slidable-micro-calendar-view/tree/master/examples/SlidingCalendarViewExample).

## Props

- **`selectedDay`** _(Date)_ - selectedDay
- **`onDaySelected`**  _(callback)_ - on selected day
---

**MIT Licensed**
