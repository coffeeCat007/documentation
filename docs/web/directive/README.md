# 指令

## v-press
- 单位时间内触发一次

``` js
/**
 * 指令 v-press
 * 点击事件单位时间内只触发第一次
 * v-press[:timeout]="fn"
 * @param event 触发的事件名称 default: click
 * @param time 单位时间 default: 1000ms
 */
```

## v-debounce-click
- 对于弹框等按钮，需要在调用接口之后才关闭，可以加上防止多次点击

``` js
/*
* 指令 v-debounce-click
* value default 500ms
* 对 <buttton> <el-button> 直接使用有效
* 其余的元素需要使用 event.target.disabled 判断 或使用 pointerEvent 模式
* .pointerEvent 不可点击模式，如果父级或元素底部有点击事件，则会穿透点击到底部事件
*/
```