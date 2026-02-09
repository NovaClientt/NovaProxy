<p align="center">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" width="80" alt="Java">
</p>

<h1 align="center">🌌 NovaProxy</h1>
<h3 align="center">🔒 Private Minecraft Proxy Infrastructure</h3>

<p align="center">
  <img src="https://img.shields.io/badge/infrastructure-private-success" alt="Private Infrastructure">
  <img src="https://img.shields.io/badge/privacy-full-green" alt="Full Privacy">
  <img src="https://img.shields.io/badge/third--party-none-red" alt="No Third Party">
  <img src="https://img.shields.io/badge/status-active-blue" alt="Active">
</p>

---

## 🧠 What is NovaProxy?
<img src="https://cdn.simpleicons.org/minecraft/62B47A" width="90" alt="Minecraft">

**NovaProxy** is a fully self-hosted Minecraft proxy system.

- Proxies are **requested via our website**  
- Proxies are **assigned and managed by us**  
- Players connect **only to their assigned proxy**  
- The client IP **never leaves our infrastructure**

---

## 🌐 Request → Assign → Connect
<img src="https://cdn.simpleicons.org/cloudflare/F38020" width="90" alt="Cloudflare">

```
👤 User
│ Request proxy
▼
🌐 NovaProxy Platform
│ Assignment
▼
📦 Dedicated Proxy
│ join proxy123.novaproxy.net
▼
🖧 The Minecraft Server
```

- ❌ No third-party providers  
- ❌ No shared proxy pools  
- ✅ Fully controlled by us  

---

## 🔁 Architecture
<img src="https://cdn.simpleicons.org/nginx/009639" width="90" alt="Nginx">

**Client → Assigned Proxy → Target Server**

```
┌──────────┐
│  Client  │
└────┬─────┘
     │
     ▼
┌──────────────────┐
│   NovaProxy      │  ← our IP
│  Analysis Layer  │
│  Routing Engine  │
└────┬─────────────┘
     │
     ▼
┌──────────────┐
│ Target Server│
└──────────────┘
```

🛡️ **The target server only sees NovaProxy.**

---

## 🔍 Connection Analysis (Internal)
<img src="https://cdn.simpleicons.org/datadog/632CA6" width="90" alt="Datadog">

```
⏳ Incoming connection
  ↓
🔎 Verify proxy assignment
  ↓
🧠 Validate rules & target
  ↓
🔐 Isolate client IP
  ↓
🚀 Forward connection
```

👉 **No data leaves our infrastructure**

---

## 🔐 IP Isolation
<img src="https://cdn.simpleicons.org/letsencrypt/003A70" width="90" alt="Security">

```diff
- ❌ Client → Target Server
+ ✅ Client → NovaProxy → Target Server
```

**Target server receives:**
```
IP Address: NovaProxy
Client IP: hidden
```

---

## ⚙️ Core Features
<img src="https://cdn.simpleicons.org/settingsdotgeneral/007ACC" width="90" alt="Settings">

- 🔐 **Full client IP protection**
- 🌐 **Proxy assignment via platform**
- 🧱 **No direct client → server connections**
- 🧠 **Internal analysis & routing**
- 🖧 **Own IPs & infrastructure**
- ⚡ **Low-latency forwarding**

---

## 🛠️ Example Configuration
<img src="https://cdn.simpleicons.org/yaml/CB171E" width="90" alt="YAML">

```yaml
proxy:
  bind-ip: 0.0.0.0
  port: 25565
  assigned-via: novaproxy-platform

routing:
  mode: internal
  target-server: mc.targetserver.net

privacy:
  expose-client-ip: false
```

---

## 🔐 Security & Privacy
<img src="https://cdn.simpleicons.org/shieldsdotio/4CAF50" width="90" alt="Shield">

✔ No third-party routing  
✔ No VPN services  
✔ No shared proxy networks  
✔ Fully self-hosted  

> ⚠️ **NovaProxy is the single connection point.**

---

## 🚀 Use Cases
<img src="https://cdn.simpleicons.org/rocketdotchat/FF9800" width="90" alt="Rocket">

- 🕶️ Play without IP leaks
- 🧪 Protected server access
- 🏗️ Dedicated proxy assignments
- 🔒 Additional security layer

---

## 🗺️ Roadmap
<img src="https://cdn.simpleicons.org/openstreetmap/7EBC6F" width="90" alt="Map">

- [x] Proxy Assignment
- [x] IP Isolation
- [x] Analysis Engine
- [ ] Multi-Server Routing
- [ ] Authentication Layer
- [ ] Admin Dashboard
- [ ] Plugin API

---

## 🌌 Summary
<img src="https://cdn.simpleicons.org/eclipseide/2C2255" width="90" alt="Eclipse">

**NovaProxy is not a middleman —  
NovaProxy is the connection point.**

> Everything goes through us.

---

## 📜 License

MIT License

---

<p align="center">
  Made with 🔒 for privacy-focused Minecraft players
</p>
