## react-native-tabbar

A tabbar component for React Native

### Overview
tabbar using react-native,support android and ios,mobile bottom tab bar with more freedom.And what's more,solved the problem overflow parent hidden on the android,also it can be defined center item by itself.

### Installation

Make sure that you are in your React Native project directory and run

```javascript
npm install react-native-nav-tabbar --save
```
### Basic usage

```javascript
import TabBar from 'react-native-nav-tabbar';
<TabBar
    initialIndex={1}
    >
    <TabBar.Item
        icon={require('./images/Home.png')}
        selectedIcon={require('./images/HomeActive.png')}
        title="Home"
    >
        <View style={styles.textContent}>
            <Text style={{fontSize: 18}}>Home</Text>
        </View>
    </TabBar.Item>
    <TabBar.Item>
        <View style={styles.textContent}>
            <Text style={{fontSize: 18}}>Friends</Text>
        </View>
    </TabBar.Item>
    <TabBar.Item
        icon={require('./images/My.png')}
        selectedIcon={require('./images/MyActive.png')}
        title="Me"
    >
        <View style={styles.textContent}>
            <Text style={{fontSize: 18}}>Me</Text>
        </View>
  </TabBar.Item>
</TabBar>
```
### TabBar props

| prop | value | required/optional | description |
| --- | --- | --- | --- |
| initialIndex | integer | optional | opens the tab with the selected index |

### Item props

| prop | value | required/optional | description |
| --- | --- | --- | --- |
| icon | image source | required | the icon when item is not focus |
| selectedIcon | image source | required | the icon when item is focus |
| title | string | required | title of item |

### Examples


![](https://raw.githubusercontent.com/territoryfan/react-native-tabbar/master/screenshots/tabbar_ios.gif)
![](https://raw.githubusercontent.com/territoryfan/react-native-tabbar/master/screenshots/tabbar_android.gif)
