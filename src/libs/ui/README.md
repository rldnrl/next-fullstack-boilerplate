# 공통적으로 사용할 컴포넌트를 여기에 넣으세요.

## 다음 폴더 구조를 추천합니다

```sh
ui
├── Button
│   ├── Button.tsx
│   └── index.tsx
├── Input
│   ├── Input.tsx
│   └── index.ts
├── Select
│   ├── Select.tsx
│   └── index.tsx
├── Textarea
│   ├── Textarea.tsx
│   └── index.tsx
└── index.tsx
```

### `Button` 폴더

```tsx
// Button/Button.tsx
interface ButtonProps extends ButtonHTMLAttributes<HTMLButtonElement> {}

const Button = (props: ButtonProps) => <button {...props} />
```

```tsx
// Button/index.tsx
import Button from './Button'

export default Button
```

```tsx
// ui/index.tsx
export { default as Button } from './Button'
```
