---
title: StorageManager
slug: Web/API/StorageManager
translation_of: Web/API/StorageManager
---
{{securecontext_header}}{{SeeCompatTable}}{{APIRef("Storage")}}

[Storage API](https://developer.mozilla.org/zh-CN/docs/Web/API/Storage_API)的**`StorageManager`**接口提供了用于管理数据本地存储权限和估算可用存储空间的接口。 您可以使用{{domxref("navigator.storage")}}或{{domxref("WorkerNavigator.storage")}}对此接口进行引用。

## 方法

- {{domxref("StorageManager.estimate()")}} {{securecontext_inline}}
  - : 返回一个{{domxref("StorageEstimate")}}对象，此对象包含为你的域名预留的存储空间总大小和你已经使用的存储空间大小。
- {{domxref("StorageManager.persist()")}} {{securecontext_inline}}
  - : 如果您的 user agent 能够将你域名下的数据持久保存，那么将返回一个状态为 resolve 的{{jsxref('Promise')}}
- {{domxref("StorageManager.persisted()")}} {{securecontext_inline}}
  - : 如果您的站点已经被授予可使用数据本地存储的权限，则返回一个状态为 resolve 的{{jsxref('Promise')}}

## 规范

{{Specifications}}

## 浏览器兼容性

{{Compat("api.StorageManager")}}
