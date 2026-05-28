# 🚀 Official Developer Documentation: The Bjve Engine Ecosystem

**Bjve** is an alternative software development ecosystem and specialized engine built to create cross-platform applications without relying on traditional vanilla JavaScript files. It acts as an educational gateway for developers to master **JavaScript, HTML, CSS, Lua, and Luau**. 

The official development environment is **BJVE Studio**, a modern desktop IDE built on **Electron** and powered by the **VS Code (Monaco Editor)** architecture. You can download the desktop application at the [Official BJVE Studio Site](https://google.com).

---

## 🛠️ The Three Core Environments & Code Syntax

Bjve is divided into three execution environments, each utilizing distinct language features and custom syntax architectures.

### 1. Bjve UEVTCL (JavaScript + Lua Scripting with OpenDraw)
The **UEVTCL** environment is designed for logic handling and standalone app builds via **OpenDraw**. It handles UI generation and graphics manipulation using an object-oriented rendering context (`ctx`).

#### Official Code Example:
```javascript
BJVE.add({
  draw(ctx) {
    ctx.fillStyle = "lime";
    ctx.fillRect(50, 50, 50, 50);
  }
});
```

### 2. Bjve Studio (HTML + CSS Interface Layouts)
The **Studio** environment manages visual styling and static structural composition. It allows developers to build app interfaces using declarative markup layouts without forcing custom JavaScript wrappers for UI design.

#### Official Code Example:
```html
<div class="box">Hello Studio</div>

<style>
.box {
  width: 150px;
  height: 150px;
  background: lime;
  color: black;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
}
</style>
```

### 3. Bjve Fire (Luau + JavaScript Engine Components)
The **Fire** variant targets high-performance scripting and game logic. It utilizes an object creation pattern similar to professional engines like Roblox via the `Instance.new()` syntax.

#### Official Code Example:
```lua
print("Hello Fire")

part = Instance.new("Part")
part.name = "Block"
part.position = {x = 10, y = 20}
```
