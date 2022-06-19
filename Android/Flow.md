# Flow
## [A safer way to collect flows from Android UIs](https://medium.com/androiddevelopers/a-safer-way-to-collect-flows-from-android-uis-23080b1f8bda)

## [Jetpack Compose 에서 Flow 효율적으로 수집하기](https://sungbin.land/jetpack-compose%EC%97%90%EC%84%9C-flow-%ED%9A%A8%EC%9C%A8%EC%A0%81%EC%9C%BC%EB%A1%9C-%EC%88%98%EC%A7%91%ED%95%98%EA%B8%B0-661fef213ced)
Hot flow나 buffer를 사용하는 flow를 UI에서 `collect` 시, 컬렉터가 없는데도 업스트림에서 데이터를 발생시키며 리소스 낭비가 발생할 수 있습니다.
그에 대한 대응으로 위 [A safer way to collect flows from Android UIs](https://medium.com/androiddevelopers/a-safer-way-to-collect-flows-from-android-uis-23080b1f8bda) 아티클에서 소개하는 `repeatOnLifecycle` 등의 API를 사용할 수 있습니다.</br>
Jetpack Compose에서는 UI에서 데이터를 수집하기 위해 flow에 대해 `collectAsState` 메서드를 사용합니다.
이를 안전하게 수집하기 위한 방법을 아티클에서 소개합니다.
