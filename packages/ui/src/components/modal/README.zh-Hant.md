---
title: 对话框
---

## API

### DDrawerProps

继承 `React.HTMLAttributes<HTMLDivElement>`。

<!-- prettier-ignore-start -->
| 参数 | 说明 | 类型 | 默认值 | 
| --- | --- | --- | --- | 
| dVisible | 抽屉是否可见 | [boolean, Updater\<boolean\>?] | - |
| dContainer | 抽屉的挂载节点, `false` 表示挂载在当前节点 | [DElementSelector](/components/Interface#DElementSelector) \| false | - |
| dPlacement | 抽屉弹出方向 | 'top' \| 'right' \| 'bottom' \| 'left'  | 'right' |
| dWidth | 抽屉宽度 | number \| string | 400 |
| dHeight | 抽屉高度 | number \| string | 280 |
| dZIndex | 手动控制 `z-index` 的值 | number \| string | - |
| dMask | 是否显示遮罩 | boolean | true |
| dMaskClosable | 点击遮罩关闭抽屉 | boolean | true |
| dEscClosable | 按下Esc是否关闭 | boolean | true |
| dHeader | 抽屉的页头 | React.ReactNode | - |
| dFooter | 抽屉的页脚 | React.ReactNode | - |
| dChildDrawer | 嵌套子抽屉 | React.ReactNode | - |
| onClose | 抽屉关闭时的回调 | `() => void` | - |
| afterVisibleChange | 抽屉打开/关闭动画结束的回调 | `(visible: boolean) => void` | - |
<!-- prettier-ignore-end -->

### DDrawerHeaderProps

等于 `Omit<DHeaderProps, 'onClose'>`。

请参考 [DHeaderProps](/components/Interface#DHeaderProps)。

### DDrawerFooterProps

继承 `DFooterProps`。

请参考 [DFooterProps](/components/Interface#DFooterProps)。

<!-- prettier-ignore-start -->
| 参数 | 说明 | 类型 | 默认值 |
| --- | --- | --- | --- |
| onOkClick | 点击确定按钮的回调，操作反馈取决于返回值，可通过 `Promise` 实现异步操作 | `() => void \| boolean \| Promise<void \| boolean>` | - |
| onCancelClick | 点击取消按钮的回调，操作反馈取决于返回值，可通过 `Promise` 实现异步操作 | `() => void \| boolean \| Promise<void \| boolean>` | - |
<!-- prettier-ignore-end -->