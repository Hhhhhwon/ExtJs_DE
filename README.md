# Ext JS 프로젝트 설정 및 실행 가이드 🌟

## 🛠 설치 및 설정
1. **Sencha Cmd 설치**: [www.sencha.com](www.sencha.com)에서 Cmd 버전에 맞게 다운로드 후 설치. 📥
2. **설치 확인**: 커맨드 라인에서 `sencha` 입력, `Sencha Cmd v7.0.0.40` 출력 확인. ✔️
3. **프로젝트 디렉토리 설정**: 
   - `dev/04.SW/10 EXT-JS/ext-js-all/ext-7.0` 경로 생성. 📁
   - `C:\SenchaSdk` 폴더 생성 후, `ext-7.0` 압축 해제. 🗂️
   - `C:\WorkspaceExtjs` 폴더 생성. 🚧

## 🚀 프로젝트 생성 및 실행
1. **HelloWorld 앱 생성**: 
   - Cmd에서 `sencha -sdk c:\senchasdk generate app HelloWorld .\HelloWorld` 실행. 🌈
2. **서버 시작 및 접속 확인**:
   - `cd HelloWorld` 후, `sencha web start` 실행. 🌐
   - `localhost:1841`에서 앱이 정상적으로 실행되는지 확인. ✅

## 🔧 테스트 기반 설정
- **app.json 수정**: `requires`에 `"font-awesome"`와 `"charts"` 추가. 📊
- **테마 변경**: Ctrl + F로 `theme` 검색 후, 원하는 테마로 변경. 예) `"theme": "theme-classic"`. 🎨

## 📦 빌드 및 배포
- **빌드 모드**: `development`, `test`, `production`. 🛠️
- **개발 환경**: 
  - 빌드 없이 소스 수정으로 바로 반영. 🔄
- **빌드 시**:
  1. 프로젝트 생성. 🌱
  2. `sencha app build development`로 로컬에서 빌드. 🏗️
  3. 개발서버에 배포. 🚀
  4. 깃허브나 형상관리 도구를 이용한 배포. 🌐
  5. 개발서버에서 바로 반영 확인. ✨
- **빌드하지 않을 경우**:
  - 로컬 개발 후 개발서버로 직접 배포. 👨‍💻
  - 운영서버에는 운영용 라이브러리로 교체하여 사용. 🔄

## 💡 추가 팁
- **Ext JS 컴포넌트**: 다양한 컴포넌트 사용 가능. [공식 문서](https://docs.sencha.com/extjs/7.0.0/classic/Ext.form.field.Date.html) 참조. 🔍
- **DOM 사용 주의**: `div-div-div` 구조로 인해 레이아웃 구성 시 주의 필요. 🚧
---


# 프로젝트 개발환경 실습 가이드 🚀

## 준비 작업 🛠

### 1. Sencha Cmd 설치 확인 ✔️
- [Sencha 공식 사이트](https://www.sencha.com/products/extjs/cmd-download/)에서 Sencha Cmd를 다운로드하고 설치합니다.
- 설치 후, 커맨드 라인에서 `sencha`를 입력하여 `Sencha Cmd v7.0.0.40`과 같은 버전 정보가 출력되는지 확인합니다.

2. **디렉토리 설정** 📁
   - 예시 입니다 -> `dev` > `04.SW` > `10 EXT-JS` > `ext-js-all` > `ext-7.0` 경로로 이동
   - `C:\SenchaSdk` 폴더 생성 후 `ext-7.0` 압축 해제
   - `C:\WorkspaceExtjs` 폴더 생성.

   3. **애플리케이션 생성 명령어 실행** 🌟
   - 커맨드 라인에서 `sencha -sdk c:\SenchaSdk generate app classic BasicClassicApp ./BasicClassicApp` 입력
     - `sencha -sdk c:\SenchaSdk`: Sencha Cmd에게 Ext JS SDK의 위치 지정
     - `generate app`: 새 애플리케이션 생성 명령
     - `classic`: 'classic' 툴킷으로 애플리케이션 생성. 데스크탑 브라우저에 최적화된 인터페이스 제공
     - `BasicClassicApp`: 생성할 애플리케이션 이름
     - `./BasicClassicApp`: 애플리케이션을 생성할 디렉토리 지정. 현재 위치(`C:\WorkspaceExtjs`)에 `BasicClassicApp` 폴더 생성 후, 애플리케이션 파일 저장
     #### 이 과정을 통해, 개발자는 Ext JS 프레임워크를 기반으로 한 새로운 웹 애플리케이션의 기본 구조를 빠르게 준비하고 시작할 수 있음.
4. **툴킷이란?** ✔️

#### 툴킷(toolkit)은 특정 작업이나 개발 과정을 지원하기 위해 필요한 도구, 라이브러리, 함수 등의 집합입니다. 소프트웨어 개발에서 툴킷은 개발자가 특정 플랫폼이나 기술 스택에서 애플리케이션을 더 효율적으로 개발할 수 있도록 돕는 다양한 도구와 구성 요소를 제공합니다.

### Sencha Ext JS 툴킷 예시 🌟

- **Classic 툴킷**:
  - 주로 데스크탑 웹 애플리케이션 개발에 최적화되어 있습니다.
  - 풍부한 UI와 복잡한 인터페이스를 지원합니다.
  - 예: `sencha -sdk c:\SenchaSdk generate app classic BasicClassicApp ./BasicClassicApp`

- **Modern 툴킷**:
  - 모바일 및 태블릿 같은 터치 기반 장치를 위해 설계되었습니다.
  - 경량화되고 반응형 디자인을 제공하여 모바일 장치의 성능과 사용자 경험을 최적화합니다.

#### Sencha Ext JS는 'classic'과 'modern'과 같은 툴킷을 제공하여 각각 데스크탑과 모바일 환경에 최적화된 웹 애플리케이션 개발을 지원합니다. 이를 통해 개발자는 상황에 맞는 최적의 애플리케이션을 빠르고 효율적으로 구축할 수 있습니다.

## 애플리케이션 빌드 및 실행 🚀
1. **프로젝트 폴더로 이동 후 빌드** 📂
   - 생성된 애플리케이션 폴더로 이동 후, 개발 모드로 빌드합니다.
     ```cmd
     C:\WorkspaceExtjs> cd BasicClassicApp
     C:\WorkspaceExtjs\BasicClassicApp> sencha app build development
     ```

2. **톰캣 서버 실행** 🖥️
   - 톰캣 서버를 시작합니다. (`startup.bat` 또는 `startup.sh` 실행)

3. **애플리케이션 배포** 📦
   - `BasicClassicApp` 폴더 내 모든 항목을 톰캣의 `webapps\ROOT` 폴더에 복사 후, 브라우저에서 `localhost:8080`으로 접속해 정상적으로 작동하는지 확인합니다.

## 주요 구성 요소와 실행 흐름 🔍
- **`index.html`**: 첫 번째로 호출되는 파일입니다. 여기서는 `bootstrap.js`를 로드합니다. 📄
- **`bootstrap.js`**: 애플리케이션에 필요한 리소스를 로드합니다. 설정은 `bootstrap.json`에서 읽어옵니다. 🔄
- **`app.js`**: `BasicClassicApp` 애플리케이션의 메인 파일입니다. Ext JS의 구조상 모든 화면은 자바스크립트 객체로 구현되어 있어 상속 구조로 개발이 가능합니다. 💡
- **실행 흐름**: `index.html` -> `bootstrap.js` -> `bootstrap.json` -> `app.js` -> mainview 호출 (`BasicClassicApp.view.main.Main`) 🛤️

# ExtJS 프로젝트 배포 프로세스 🚀

## 프로덕션 빌드 및 배포 준비 🛠

- **톰캣 서버 준비**: 
  - `tomcat/webapps`에서 `app`, `resource` 폴더를 `BasicClassicApp` 프로젝트 폴더로 복사합니다.
  
- **프로덕션 모드 빌드**: 
  ```bash
  cd BasicClassicApp sencha app build production
  ```
- `build/production`: 폴더 내에 빌드된 애플리케이션(`BasicClassicApp`)이 생성됩니다.

-**리소스 관리**:

- `resource` 📂에는 이미지나 필요한 라이브러리를 관리합니다. 이미지는 images 폴더에 별도로 관리됩니다.

### 배포 준비 📦

1. **프로덕션 폴더 확인**: `build/production/BasicClassicApp` 내에 생성된 파일들을 확인합니다.
2. **운영 서버 준비**: 현재 운영 서버가 없는 경우, 개발 목적으로 사용 중인 톰캣 서버를 운영 서버로 간주할 수 있습니다.

### 배포 실행 🌐

1. **톰캣 서버의 `webapps/ROOT` 폴더로 이동**: `BasicClassicApp` 폴더 내의 모든 내용을 톰캣 서버의 `webapps/ROOT` 폴더에 복사합니다.
   - 이 과정은 실제 운영 환경에서 애플리케이션을 배포할 때와 유사합니다.
2. **톰캣 서버 재시작**: 변경사항을 적용하기 위해 톰캣 서버를 재시작합니다.

### 결과 확인  ✅

브라우저에서 `localhost:8080` 주소로 접속하여, 프로덕션 환경에서의 애플리케이션 작동 여부를 확인합니다. 이 단계에서 애플리케이션이 정상적으로 로드되고 작동한다면, 프로덕션 빌드 및 배포 과정이 성공적으로 완료된 것입니다.

### 주의사항 🚨

- **운영 서버가 없는 경우의 대안**: 지금 가이드 에서는 운영 서버가 없는 경우 개발 서버를 임시로 사용하는 방법을 제시하고 있습니다. 실제 운영 환경에서는 보안, 성능, 관리 측면을 고려하여 적절한 운영 서버 구성이 필요합니다.
- **파일 관리**: 프로덕션 빌드 과정에서 생성된 파일들은 최적화되고 난독화되어 있으므로, 소스 코드의 수정 및 관리는 개발 환경에서 이루어져야 합니다.

# ExtJS 프로젝트 최종 배포 과정 🚀

## 배포 준비
- 톰캣 서버의 `webapps/ROOT` 폴더로 이동합니다. 여기서는 `WEB-INF` 폴더를 제외한 모든 파일과 폴더를 삭제합니다. 이는 프로덕션 환경을 깨끗하게 준비하기 위함입니다.

## 프로덕션 모드 빌드
- 프로젝트 폴더에서 다음 명령어를 실행하여 프로덕션 모드로 애플리케이션을 빌드합니다:
  ```bash
  cd BasicClassicApp && sencha app build production
  ```
  ## 애플리케이션 배포 🌐
- `build/production/BasicClassicApp` 폴더 안의 내용을 톰캣의 `webapps/ROOT` 폴더에 복사합니다.
- 톰캣 서버를 재시작하여 변경사항을 적용합니다.

## 변경 사항 확인 ✅
- 브라우저에서 `localhost:8080` 주소로 접속하여 애플리케이션이 정상적으로 작동하는지 확인합니다.

## 프로덕션 모드의 특징 🌟
- `app` 폴더가 사라지고, 모든 JavaScript 파일이 `app.js`로 합쳐지고 난독화됩니다.
- `ext-all.js` 또는 `ext-rtl-all.js`를 사용하며, 개발 모드에서 사용되던 `ext-all-debug.js` 또는 `ext-all-rtl-debug.js`는 사용되지 않습니다.
- 소스 코드의 수정 및 관리는 개발 모드에서 이루어져야 하며, 필요한 변경사항은 개발 모드에서 적용한 후 다시 빌드해야 합니다.

## 추가 팁 💡
- Ext JS의 `ext-all.js`와 `ext-all-debug.js` 파일에 대한 설명:
  - `ext-all.js`: Ext JS의 모든 컴포넌트를 포함한 압축된 파일로, 프로덕션 환경에서 사용됩니다.
  - `ext-all-debug.js`: 동일한 컴포넌트를 포함하지만 압축되지 않고, 디버깅을 용이하게 하는 주석과 함께 제공됩니다.
- 프로덕션 빌드된 후 `index.html`이 호출하는 구조가 변경될 수 있으므로, 주의가 필요합니다.

## Ext JS의 `ext-all.js`와 `ext-all-debug.js` 파일 설명 📚

- **`ext-all.js`**:
  - Ext JS의 모든 컴포넌트를 포함한 압축된 파일입니다.
  - 프로덕션 환경에서 사용됩니다.
  - 애플리케이션의 로딩 시간을 최소화하기 위해 압축된 형태로 제공됩니다.

- **`ext-all-debug.js`**:
  - `ext-all.js`와 동일한 컴포넌트를 포함하지만, 압축되지 않은 상태입니다.
  - 개발 중에 디버깅을 용이하게 하는 주석과 함께 제공됩니다.
  - 개발자가 코드를 쉽게 이해하고 문제를 진단할 수 있도록 설계되었습니다.

- **`ext-all-rtl-debug.js`**:
  - 오른쪽에서 왼쪽으로(RTL) 읽는 언어를 지원하기 위한 디버그 파일입니다.
  - RTL 지원이 필요한 애플리케이션 개발 시 사용됩니다.
  - 개발 환경에서 `ext-all-debug.js`와 함께 RTL 디버깅을 지원합니다.

### 일반적인 사용 방법 🔄
- 개발 시에는 `ext-all-debug.js` 또는 `ext-all-rtl-debug.js`를 사용하여 애플리케이션의 동작을 확인하고 디버깅합니다.
- 프로덕션 환경에서는 압축된 `ext-all.js`를 사용하여 애플리케이션의 로딩 시간을 개선하고, 네트워크 전송 시간을 줄입니다.











