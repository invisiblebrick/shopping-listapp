# 🛒 Shopping List App

간단하고 사용하기 쉬운 쇼핑 리스트 웹 애플리케이션입니다.

## ✨ 주요 기능

- **아이템 추가**: 입력창에 아이템을 입력하고 '추가' 버튼 또는 Enter 키로 추가
- **체크 기능**: 각 아이템 앞의 체크박스를 클릭하여 완료 표시
- **아이템 삭제**: 각 아이템의 '삭제' 버튼으로 개별 삭제
- **전체 삭제**: 하단의 '전체 삭제' 버튼으로 모든 아이템 삭제
- **데이터 저장**: 로컬 스토리지를 사용하여 브라우저를 닫아도 데이터 유지
- **반응형 디자인**: 모바일과 데스크톱 모두 지원

## 🔒 보안 개선 사항

- **XSS 방어**: `innerHTML` 대신 `textContent`와 `createElement()` 사용으로 XSS 공격 차단
- **이벤트 핸들링**: 인라인 이벤트 핸들러 제거, `addEventListener()` 사용
- **에러 핸들링**: localStorage 접근 실패 시 안전한 폴백 처리
- **최신 API**: deprecated된 `keypress` 이벤트 대신 `keydown` 사용

## 🚀 사용 방법

1. 저장소를 클론하거나 `index.html` 파일을 다운로드하세요
2. 브라우저에서 `index.html` 파일을 열어주세요
3. 별도의 설치나 서버 없이 바로 사용 가능합니다!

## 💻 기술 스택

- **HTML5**: 구조적인 마크업
- **CSS3**: 반응형 디자인, 애니메이션
- **Vanilla JavaScript (ES6+)**: 프레임워크 없이 순수 JavaScript로 구현
- **localStorage API**: 클라이언트 측 데이터 영속성

## 📝 라이선스

MIT License

## 🧪 테스트

Playwright를 사용한 자동화 테스트 완료:
- ✅ 아이템 추가 기능
- ✅ 체크박스 토글 기능
- ✅ 개별/전체 삭제 기능
- ✅ XSS 보안 검증

---

**Live Demo**: [GitHub Pages에서 확인하기](https://invisiblebrick.github.io/shopping-listapp/)