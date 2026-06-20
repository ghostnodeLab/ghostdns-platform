# 🚀 GhostDNS · 多租户子域名与流量路由平台

> 下一代子域名与 DNS 路由管理平台（面向开发者与 SaaS 构建者）

🌐 在线演示：https://yourdns.ghostnode.dev  
📦 项目状态：生产级可用  
⚡ 架构模式：多租户 DNS + 流量路由系统

---

## ✨ GhostDNS 是什么？

GhostDNS 是一个现代化的基础设施平台，用于快速构建：

- 子域名分发系统
- 多用户 DNS 管理平台
- 流量代理与跳转系统
- SaaS 多租户域名服务

它可以帮助开发者快速搭建类似：

- SaaS 平台域名系统  
- 开发者工具平台  
- 多用户子域名服务  
- 链接分发与跳转系统  

---

## ⚡ 核心能力

### 🆓 免费子域名系统
- 即时子域名分配
- 基于泛解析架构（*.domain.com）
- 无需手动创建 DNS 记录
- 自动进入代理路由系统

---

### 💎 高级域名系统（付费）
- 关键词级别识别（Premium Words）
- USDT 手动支付流程
- 管理员审核机制
- 域名生命周期管理（生效 / 过期 / 禁用）

---

### 🌐 真实 DNS 管理系统（Cloudflare）
支持完整 DNS 记录管理：

- A 记录
- AAAA 记录
- CNAME 记录
- TXT 记录

功能包括：

- TTL 校验
- 用户配额限制
- 管理员控制开关
- Cloudflare API 自动写入

---

### 🔁 智能路由系统

每个域名支持动态路由：

- 🟢 代理模式 → 转发到目标站点  
- 🔵 跳转模式 → 302 重定向  
- ⚪ 停放模式 → 展示默认页面  
- 🔴 禁用状态 → 拒绝访问  

---

### 📧 邮件系统
- 邮箱验证
- 找回密码
- 系统通知
- 支持：
  - SMTP
  - Brevo
  - Resend（推荐）

---

### 🛡 安全与风控系统
- SSRF 防护机制
- IP / 域名访问频率限制（Redis 支持）
- 滥用举报系统
- 保留词 / 高级词保护
- 完整操作日志审计

---

### 💰 商业化能力
- USDT 手动支付系统
- 订单生命周期管理
- 管理员审核后台
- 灵活定价策略
- 高级域名升级机制

---

## 🧠 系统架构

```
用户访问
     ↓
Cloudflare 泛解析 (*.domain.com)
     ↓
GhostDNS 代理层
     ↓
路由引擎
     ├── 代理转发（Proxy）
     ├── 302 跳转（Redirect）
     ├── 停放页面（Parking）
     └── 支付提示页面
```

---

## 🧩 技术栈

- Next.js 14+
- TypeScript
- PostgreSQL
- Prisma ORM
- Redis（可选）
- Cloudflare API
- Nginx / 反向代理
- Docker

---

## 🚀 快速启动

```bash
git clone https://github.com/yourname/ghostdns
cd ghostdns

npm install
cp .env.example .env

npm run dev
```

---

## ⚙️ 生产环境部署

```bash
npm run build
npm run start
```

Docker 部署：

```bash
docker compose up -d --build
```

---

## 🌍 使用示例

```
https://demo.yourdomain.com
https://app.yourdomain.com
https://test.yourdomain.com
```

---

## 🔥 适用场景

- SaaS 平台构建
- 开发者工具平台
- 多租户系统
- 链接分发系统
- 域名交易平台
- 企业级子域名管理系统

---

## 🧠 为什么选择 GhostDNS？

传统 DNS 系统：

❌ 静态配置  
❌ 管理复杂  
❌ 不支持多租户  
❌ 无商业化能力  

GhostDNS：

✅ 动态路由  
✅ 多用户架构  
✅ 内置商业模型  
✅ Cloudflare 原生支持  
✅ 可直接生产部署  

---

## 🌐 在线体验

👉 https://yourdns.ghostnode.dev

---

## 📌 注意事项

- 需要泛解析 DNS（Wildcard DNS）
- 推荐 Cloudflare
- Redis 可选但推荐
- VPS / Docker 部署环境

---

## ⚠️ 免责声明

仅用于合法基础设施与开发用途。

用户需自行负责域名使用行为。

---

## 📈 路线图

- 支付自动化（Stripe / Crypto）
- SaaS 模板市场
- 团队协作
- Open API
- 模板化子域名应用

---

## 👨‍💻 作者

GhostNode Lab  
https://ghostnode.dev

---

## 🚀 开始构建

适用于：

- SaaS 产品
- 开发者平台
- 多租户系统
- 域名服务系统
