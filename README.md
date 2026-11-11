# 킹제임스 흠정역 – Android 프로젝트
index.html 을 app/src/main/assets/ 에 넣은 WebView 앱 (완전 오프라인, targetSdk 36 / Android 16, minSdk 24).

## 방법 A. Android Studio (가장 쉬움)
1. Android Studio 로 이 폴더 열기 → Gradle Sync
2. Build > Build APK(s)
3. app/build/outputs/apk/debug/app-debug.apk 를 폰으로 복사해 설치

## 방법 B. 설치 없이 GitHub에서 빌드
1. 이 폴더 전체를 새 GitHub 저장소에 업로드
2. Actions 탭 > Build APK 실행 완료 후 Artifacts 에서 apk 다운로드

## 방법 C. 명령줄
JDK17 + Android SDK(platform 36) 설치 후:  gradle assembleDebug
