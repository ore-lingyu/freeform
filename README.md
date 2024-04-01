# freeform
1、有5个patch<br>
bounds.patch    ---这个是自由窗口拖动放大缩小只操作Task SurfaceControl的核心部分<br>
TaskResizingAlgorithm.patch  ---这个是Task区域外等比例放大缩小窗口SurfaceControl的 数学计算部分<br>
ShellDragResize.patch  ---这个是解决r24版本 Task区域外拖动事件被拦截的问题<br>
freeform_animation_remove.patch  ---这个是解决进入自由窗口由于动画播放导致的闪屏问题<br>
freeform_stoke_draw.patch    ---这个是给自由窗口放大缩小时增加边框高亮显示<br>

2、打patch 在aosp版本 13 r24分支<br>
git apply bounds.patch<br>
git apply TaskResizingAlgorithm.patch<br>
git apply ShellDragResize.patch<br>
git apply freeform_animation_remove.patch<br>
git apply freeform_stoke_draw.patch<br>

3、FreeForm相关知识<br>
https://docs.qq.com/s/BmkanaZVOPd-zjT--B_Ojq
