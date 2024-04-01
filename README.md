# freeform
1、有5个patch
bounds.patch    ---这个是自由窗口拖动放大缩小只操作Task SurfaceControl的核心部分
TaskResizingAlgorithm.patch  ---这个是Task区域外等比例放大缩小窗口SurfaceControl的 数学计算部分
ShellDragResize.patch  ---这个是解决r24版本 Task区域外拖动事件被拦截的问题
freeform_animation_remove.patch  ---这个是解决进入自由窗口由于动画播放导致的闪屏问题
freeform_stoke_draw.patch    ---这个是给自由窗口放大缩小时增加边框高亮显示

2、打patch 在aosp版本 13 r24分支
git apply bounds.patch
git apply TaskResizingAlgorithm.patch
git apply ShellDragResize.patch
git apply freeform_animation_remove.patch
git apply freeform_stoke_draw.patch

3、FreeForm相关知识
https://docs.qq.com/s/BmkanaZVOPd-zjT--B_Ojq
