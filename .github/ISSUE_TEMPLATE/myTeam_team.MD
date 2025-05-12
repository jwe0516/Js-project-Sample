name: "기본 컨벤션"
description: "기본 컨벤션입니다."
body:

- type: checkboxes
  attributes:
  label: 🔧 PR 유형
  description: 해당하는 PR 유형을 선택하세요.
  options: - label: 새로운 기능 추가 - label: 버그 수정 - label: CSS 등 사용자 UI 디자인 변경 - label: 코드에 영향을 주지 않는 변경사항(오타 수정, 탭 사이즈 변경, 변수명 변경) - label: 코드 리팩토링 - label: 주석 추가 및 수정 - label: 문서 수정 - label: 테스트 추가, 테스트 리팩토링 - label: 빌드 부분 혹은 패키지 매니저 수정 - label: 파일 혹은 폴더명 수정 - label: 파일 혹은 폴더 삭제

- type: textarea
  attributes:
  label: 📄 PR 상세
  description: PR 내용을 적어주세요.
  placeholder: 규칙에 맞게 작성해주세요.
  validations:
  required: true

- type: checkboxes
  attributes:
  label: ✅ PR 체크리스트
  description: PR이 다음 요구 사항을 충족하는지 확인하세요.
  options: - label: 커밋 메시지 컨벤션에 맞게 작성했습니다. - label: 변경 사항에 대한 테스트를 했습니다.(버그 수정/기능에 대한 테스트).

- type: input
  attributes:
  label: 🔗 이슈
  description: 이슈 번호를 입력해주세요 (예: #1, resolves #1).
  placeholder: resolves #1
