# WelcomeFarewell

入群欢迎和退群欢送功能

## 更新日志

### 2024-11-02

- fix: 修复无法加载自定义通知消息的 bug

### 2024-10-6

- feat: 重构逻辑，分离入群欢迎和退群欢送的逻辑，单独定义
- fix: 优化数据库初始化逻辑，避免在每次处理群通知时反复初始化数据库
- feat: 优化菜单，增加功能描述和注意事项

### 2024-10-5

- feat: 删除命令中的短线，方便用户使用

### 2024-9-29

- feat: 修改入群欢迎和退群欢送的欢迎词和退群欢送词中包含 CQ 码时，CQ 码无法解析的问题

### 2024-8-25

- feat: 修改命令格式，去除空格
- fix: 修复由于上层供应链的变化，导致正则匹配失败的问题
- fix: 修复回调函数没有 json.loads 导致报错字符串不能使用 get 方法的 bug
- fix: 修复了范围限定的错误导致无法触发入群欢迎

### 2024-8-24

- feat: 限定范围，只处理入群和退群事件

### 2024-8-23

- feat: 修改命令格式，去除空格

### 2024-8-22

- feat: 增加了入群欢迎和退群欢送的欢迎词和退群欢送词的配置
- fix: 修复了入群欢迎和退群欢送的欢迎词和退群欢送词中包含 CQ 码时，CQ 码无法解析的问题

### 2024-8-21

- feat: 融合了黑名单检测，当入群时，如果用户在黑名单中，则不发送欢迎词，并且直接踢出

### 2024-8-14

- fix: 修复由于角色判断错误导致的开关失效的 bug
