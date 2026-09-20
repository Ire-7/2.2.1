# gyr · 北京最后一个秋冬 v2.2.1 Map Fix

QA 修复版：
- 修复主地图初始化时 Leaflet 尚未加载的问题
- 地图只在“足迹”页真正显示后初始化，并主动 invalidateSize
- 移除覆盖真实地图的模糊 fallback 视觉
- 增加地图状态与重试按钮
- 使用用户选定的第一版蜡笔 gyr 图作为 PWA icon 与地图测试 marker
- 没有带坐标记录时，北京中心会显示一只测试 gyr；保存真实坐标后自动替换为真实足迹
- Service Worker cache bump，减少 iOS 旧资源缓存

验收：足迹页应显示清晰可缩放地图 + 一只小 gyr；点小 gyr 有 popup。
