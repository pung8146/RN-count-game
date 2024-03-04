# boxShadow

> 그림자 효과는 ios와 android에서 다르게 적용됩니다.

## Android

> elevation 0,1,2,3... 높을 수록 그림자가 선명해진다.

## IOS

- shadowColor : 'black' : 원하는 그림자색
- shadowOffset : {width: 0, height: 2} : 그림자 위치 // 0,2는 아래로 그림자가 생김
- shadowRadius : 6 : 그림자 둥글기
- shadowOpacity : 0.26 : 그림자 투명도

# keyboardType 이란 ?

> 키보드 타입을 설정할 수 있습니다. 또한 플랫폼 구분 없이 지원되거나, 플랫폼에 따라 다르게 적용되는 속성들이 있습니다. 확인은 공식문서인 [TextInput](https://reactnative.dev/docs/textinput) - keyboardType에서 확인할 수 있습니다.

# 모든 스타일 지정하기

> app.json파일에 backgroundColor : 'white'와 같이 모든 스타일을 지정할 수 있습니다.

# LinearGradient 사용하기

## expo-linear-gradient 설치하기

1. expo install expo-linear-gradient 터미널에 입력

- npm으로 설치 않고 expo로 설치시 자동으로 Expo버전과 호환되는 버전이 설치됩니다.

2.  import { LinearGradient } from 'expo-linear-gradient'; 를 입력하여 사용할 수 있습니다.

3.  <LinearGradient> 태그를 사용하여 그라데이션을 적용할 수 있습니다.

4.  <LinearGradient colors={["#4e0329", "#ddb52f"]} > 그라데이션 색상을 지정할 수 있습니다.

# 번외 npm install -g expo-cli 가 사용되지 않는다 합니다.

# ImageBackground 사용하기

# react-native 에서 useState 사용하기

>

# TextInput 은 항상 문자열을 반환합니다.

> <TextInput keyboardType="number-pad"> 여도 결과값은 문자열로 반환됩니다.

# Alert 사용하기

1. Import {Alert} from 'react-native';

- 경고창을 표시하는 컴포넌트가 아니라 alert 메소드를 사용합니다.

2. Alert.alert or Alert.prompt 를 입력할 수 있습니다.

3. 세개의 인수를 받으며, 첫번째는 제목, 두번째는 내용, 세번째는 버튼을 배열로 받습니다.

4. Alert.alert('제목', '내용', [{text: '버튼이름', style: '' ,onPress: () => console.log('버튼을 눌렀을 때 실행할 함수')}])

5. button 객체안에서 모든 text 를 가지고 있습니다.

- style default, cancel, destructive를 가질 수 있습니다. 기본,취소,삭제 버튼을 의미합니다.
- 스타일에 따라 버튼의 색상이 굵기가 달라집니다.

# SafeAreaView 사용하기

> SafeAreaView는 ios에서 notch영역을 피하기 위해 사용됩니다.

# expo-font 사용하기

1. expo install expo-font

```jsx
import { useFonts } from "expo-font";
```

# expo-app-loading 사용하기

1. npm install expo-app-loading

```jsx
import AppLoading from "expo-app-loading";
```

# expo-splash-screen 사용하기

> expo-app-loading 대신 사용할 수 있습니다.

# Dimensions API 사용하기

> 기기의 너비와 높이를 가져올 수 있습니다.

1. import { Dimensions } from "react-native"; 네이티브에서 불러옵니다.
2. const 변수명 = Dimensions.get("window or screen") => get 메서드가 문자열 타입 인수로서 화면이나 윈도우의 치수를 가져옵니다.
3. 안드로이드에서 screen은 상태 표시줄을 포함한 너비와 높이를 가져옵니다. window는 상태 표시줄을 제외한 너비와 높이를 가져옵니다.
4. const 변수명 = Dimensions.get("window").width => .width .height로 너비와 높이를 가져올 수 있습니다.

# 화면 회전

> Expo는 기본적으로 orientation을 portrait로 설정되어 있습니다.(세로고정), landscape로 설정하면 가로고정이 됩니다. default는 기기의 설정에 따라서 화면이 회전됩니다. 이 설정은 app.json에서 설정할 수 있습니다.
