# 生产工具 「简介 + npm 地址」

## 操作 cookie [@marshal93/cookie](https://www.npmjs.com/package/@marshal93/cookie)

### Usage

```typescript
function getAllCookies(): object;

function getCookie(name: string): string | undefined;

function setCookie(name: string, value: string, extra: {
  domain?: string;
  path?: string;
  days?: number;
  encoding?: boolean;
} = {}): void;

function deleteCookie(name: string, extra: {
  domain?: string;
  path?: string;
} = {}): void;
```

## 操作 storage [@marshal93/storage](https://www.npmjs.com/package/@marshal93/storage)

### Usage
```js
import storageFactory from '@marshal93/storage';

const storage = storageFactory(`${app_name}@${user_id}`); // 默认 locationStorage
const session = storageFactory(`${app_name}@${user_id}`, true); // 如果还需要 sessionStorage 的操作，可以这样

storage(); // 获取全部
storage(key); // 获取某个值
storage(key, val); // 设置某值
storage(key, null); // 清除某值
```

## 复制文本 [@marshal93/copy-text](https://www.npmjs.com/package/@marshal93/copy-text)

### Usage
```typescript
import copyText from '@marshal93/copy-text';

copyText(...some...text...);
```

----

# 开发环境工具「简介 + npm 地址」

## 自定义 eslint [@marshal93/eslint-config](https://www.npmjs.com/package/@marshal93/eslint-config)

### es5
```json
{
  "extends": [
    "@marshal93/eslint-config/es5"
  ]
}
```

### es6
```json
{
  "extends": [
    "@marshal93/eslint-config/es6"
  ]
}
```

### react
```json
{
  "extends": [
    "@marshal93/eslint-config/react"
  ]
}
```

### ts / tsx 项目
```json
{
  "extends": [
    "@marshal93/eslint-config/ts"
  ]
}
```

```json
{
  "extends": [
    "@marshal93/eslint-config/tsx"
  ]
}
```

## 自定义 stylelint [@marshal93/stylelint-config](https://www.npmjs.com/package/@marshal93/stylelint-config)

### Usage

```json
{
  "extends": [
    "@marshal93/stylelint-config"
  ]
}
```
