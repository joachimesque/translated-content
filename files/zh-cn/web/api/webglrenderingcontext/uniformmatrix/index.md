---
title: WebGLRenderingContext.uniformMatrix[234]fv()
slug: Web/API/WebGLRenderingContext/uniformMatrix
tags:
  - WebGL
  - WebGLAPI
  - WebGLRenderingContext
  - uniformMatrix2fv
  - uniformMatrix3fv
  - uniformMatrix4fv
  - 矩阵
translation_of: Web/API/WebGLRenderingContext/uniformMatrix
---
{{APIRef("WebGL")}}

[WebGL API](/en-US/docs/Web/API/WebGL_API) 的**`WebGLRenderingContext.uniformMatrix[234]fv()`** 方法为 uniform variables 指定了矩阵值 .

该方法的 3 个版本 (`uniformMatrix2fv()`, `uniformMatrix3fv()`, 和`unifomMatrix4fv()`) ,分别以二阶，三阶，和四阶方阵作为输入值，它们应是分别具有 4,9,16 个浮点数的数组。

## 语法

```plain
WebGLRenderingContext.uniformMatrix2fv(location, transpose, value);
WebGLRenderingContext.uniformMatrix3fv(location, transpose, value);
WebGLRenderingContext.uniformMatrix4fv(location, transpose, value);
```

### 参数

- `location`
  - : {{domxref("WebGLUniformLocation")}} 对象包含了要修改的 uniform attribute 位置。位置使用 {{domxref("WebGLRenderingContext.getUniformLocation", "getUniformLocation()")}}获得。
- `transpose`
  - : {{domxref("GLboolean")}} 指定是否转置矩阵。必须为 `false`.
- `value`
  - : {{jsxref("Float32Array")}} 型或者是 `GLfloat` 序列值。假定值以列主要顺序提供。

### 返回值

`undefined`

## 示例

```js
gl.uniformMatrix2fv(loc, false, [2,1, 2,2]);
```

## 规范

{{Specifications}}

## 浏览器兼容性

{{Compat("api.WebGLRenderingContext.uniformMatrix2fv")}}

## 另见

- {{domxref("WebGLRenderingContext.uniform()")}}
- {{domxref("WebGL2RenderingContext.uniformMatrix()")}} – WebGL 2 versions of these methods.
