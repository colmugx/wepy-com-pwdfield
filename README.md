# wepy-com-pwdfield

[![NPM](https://nodei.co/npm/wepy-com-pwdfield.png)](https://nodei.co/npm/wepy-com-pwdfield/)

> 适用于房间号输入，验证码输入，密码等有位数限制明密文输入框


![](/screenshot/1.gif)

## 安装 Install

> npm install -S wepy-com-pwdfield

## 使用 Usage

```js
import Pwdfield from 'wepy-com-pwdfield'

export ...

    components = {
      pwdfield: Pwdfield
    }
```

```vue
<pwdfield :sixdig="sixdig" :display="display" color="#444751" @value="handleValue" />
```
默认是选择数字，从`1`到`4`，颜色是`#444751`

## 配置 Options

### Api

| 参数       | 说明               | 类型              | 可选值         | 默认值     |
| -------- | ---------------- | --------------- | ----------- | ------- |
| sixdig    | 开启六位数 | Boolean | -           | -       | false
| display    | 明密文         | Boolean        | -           | true       |
| color  | 边框颜色           | String          | -           | #444751 |

### Event

| 参数        | 说明       | 返回值              |
| --------- | -------- | ---------------- |
| value | 实时获取填写变化 | String |
