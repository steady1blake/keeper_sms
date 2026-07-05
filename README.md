# 키퍼 CCTV 문자/견적서 템플릿

한화비전 키퍼 CCTV 인바운드 상담용 문자 템플릿 + 정식견적서(가로 PNG) 생성 도구.

## 사용 방법
`index.html`을 브라우저로 열면 바로 동작합니다. 서버/빌드 과정이 필요 없는 순수 정적 페이지입니다.

## 담당자 추가/수정
`index.html` 안의 `STAFF` 객체(스크립트 상단)에서 이름과 연락처를 관리합니다.

```js
const STAFF = {
  '구태진': { name: '구태진', mobile: '010-2861-3385' },
  '김수정': { name: '김수정', mobile: '010-2765-9766' }
};
```

새 담당자를 추가하려면:
1. 위 `STAFF` 객체에 항목 추가
2. 상단 담당자 선택 버튼 영역(`<div class="staff-tabs" id="staffTabs">`)에 버튼 한 줄 추가

## 배포 (Vercel)
이 폴더를 GitHub에 올리고 Vercel에서 그대로 Import하면 별도 빌드 설정 없이 배포됩니다 (정적 HTML이라 Framework Preset: **Other** 선택).
