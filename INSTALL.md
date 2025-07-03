项目配置
依赖环境：

现代浏览器（Chrome/Firefox/Edge 最新版）

无需后端服务器（数据存储在浏览器本地）

文件结构：

text
demo15.html        # 主程序文件
关键配置项：

本地存储键名（可在代码中修改）：

javascript
storageKey: 'canteen_windows_data',   // 窗口数据存储
orderKey: 'canteen_windows_order',    // 卡片排序存储
favoritesKey: 'canteen_my_favorites'  // 收藏窗口存储
编译说明
🛠️ 本项目为纯前端静态页面，无需编译

所有代码（HTML/CSS/JavaScript）已内联在 demo15.html 中

直接通过浏览器运行即可

安装与运行
方法1：直接浏览器打开
双击 demo15.html 文件

浏览器自动加载页面

方法2：本地服务器运行（推荐）
bash
# 安装简单 HTTP 服务器（Node.js 环境）
npm install -g http-server

# 进入项目目录
http-server -p 8080
访问：http://localhost:8080/demo15.html

方法3：Python 简易服务器
bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
访问：http://localhost:8000/demo15.html

功能验证
用户端功能：

✅ 实时食堂窗口数据展示

✅ "我常吃的" 窗口收藏（拖拽排序）

✅ 拥挤度分析/高峰期预测

✅ 商家公告查看

商家端功能：

✅ 切换管理窗口

✅ 发布/删除公告

✅ 回复用户评论

特色交互：

✨ Magic模式：启用动态拖拽/果冻动画

📊 数据本地持久化（刷新页面不丢失）

注意事项
所有数据存储在浏览器 localStorage 中

清除浏览器缓存将重置数据

模拟数据每分钟自动更新一次

商家切换功能在右上角角色切换区

项目完整代码已内联在单文件中，无需额外文件支持。
