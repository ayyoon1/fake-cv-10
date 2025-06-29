# Fake CV 프로젝트

이 프로젝트는 `index.html`과 순수 JavaScript(Vanilla JS)를 사용하여 만든 동적 이력서(CV) 웹사이트입니다. 모든 데이터는 JavaScript 객체에서 관리되며, 이를 통해 쉽게 자신의 정보로 교체하고 맞춤화할 수 있습니다.

## ✨ 주요 기능

-   **데이터 기반 동적 렌더링**: `js/data.js` 파일에 있는 데이터 객체를 기반으로 모든 컨텐츠가 동적으로 생성됩니다.
-   **다국어 지원 (한/영)**: 버튼 클릭으로 한국어와 영어 버전을 실시간으로 전환할 수 있습니다.
-   **모듈화된 구조**: 자기소개, 학력, 경력, 프로젝트, 기술 등 각 섹션이 명확하게 구분되어 있습니다.
-   **쉬운 커스터마이징**: `js/data.js` 파일만 수정하면 자신의 이력서로 쉽게 변경할 수 있습니다.
-   **순수 JS 구현**: 외부 라이브러리나 프레임워크 없이 순수 HTML, CSS, JavaScript로만 제작되었습니다.

## 📁 프로젝트 구조

```
.
├── assets/
│   └── images/
│       ├── profile.png
│       └── projects/
│           ├── project1.png
│           ├── project2.png
│           └── project3.png
├── css/
│   └── style.css
├── js/
│   ├── data.js     # 이력서 데이터 (이 파일만 수정하면 됩니다)
│   └── script.js   # 동적 렌더링 로직
├── index.html      # 메인 HTML 파일
└── README.md
```

## 🛠️ 사용법 및 커스터마이징

이 이력서를 자신의 것으로 만들려면 다음 단계를 따르세요.

1.  **프로필 이미지 변경**: `assets/images/profile.png` 파일을 자신의 사진으로 교체합니다.
2.  **프로젝트 썸네일 추가**: `assets/images/projects/` 디렉토리에 프로젝트 관련 이미지를 추가합니다.
3.  **데이터 수정**: `js/data.js` 파일을 열어 `cvData` 객체의 내용을 자신의 정보로 수정합니다. 이름, 연락처, 자기소개, 학력, 경력, 프로젝트, 기술 스택 등 모든 정보를 이곳에서 관리합니다.

    ```javascript
    // js/data.js

    const cvData = {
      personalInfo: {
        name: {
          kor: "홍길동", // 본인 이름으로 수정
          eng: "Gildong Hong",
        },
        // ... 기타 모든 정보 수정
      },
      // ...
    };
    ```

4.  **브라우저에서 확인**: `index.html` 파일을 웹 브라우저에서 열어 변경사항을 확인합니다.

## 🚀 기술 스택

-   HTML5
-   CSS3
-   JavaScript (ES6+)
