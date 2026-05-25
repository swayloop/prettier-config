# @swayloop/prettier-config

swayloop org 공통 Prettier 포매팅 설정.

## 설치

```bash
pnpm add -D @swayloop/prettier-config prettier
```

## 사용

`package.json` 에 한 줄 추가:

```json
{
  "prettier": "@swayloop/prettier-config"
}
```

별도 `.prettierrc` 파일 없이도 동작. 커스텀이 필요하면 `.prettierrc.js`:

```js
module.exports = {
  ...require('@swayloop/prettier-config'),
  // 프로젝트별 오버라이드
  printWidth: 120,
};
```

## 포함된 옵션

| 옵션 | 값 |
|---|---|
| `singleQuote` | `true` |
| `semi` | `true` |
| `trailingComma` | `"all"` |
| `printWidth` | `100` |
| `tabWidth` | `2` |
| `useTabs` | `false` |
| `arrowParens` | `"always"` |
| `endOfLine` | `"lf"` |
| `bracketSpacing` | `true` |

## 표준

브랜치/커밋/릴리즈 규칙은 [swayloop/.github](https://github.com/swayloop/.github/blob/main/docs/workflow.md) 참고.
