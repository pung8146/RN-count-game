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
