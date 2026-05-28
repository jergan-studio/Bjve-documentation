# 📖 Bjve Language Engine: Complete Core Documentation

Welcome to the comprehensive technical manual for the **Bjve programming language** ecosystem. Bjve is an independent, native scripting language engineered to construct cross-platform applications without relying on traditional, complex web script stacks. 

This document serves as the absolute source of truth for syntax rules, engine frameworks, and architecture compilation.

---

## ⚡ 1. Global Syntax & Universal Commands

The Bjve runtime engine maintains a unified global scope shared across all execution sub-engines. Every runtime variant natively supports the global thread dialog hook:

```bjve
alert("gameoverse")
```

### ⚙️ Engine Thread Behavior:
* Calling `alert()` instantly interrupts active execution blocks and freezes processing threads.
* It commands the desktop IDE core window wrapper to blit a native system dialogue window displaying the targeted string payload.
* Use double quotes `"`, single quotes `'`, or string template literals to enclose message values.

---

## 🎨 2. Bjve UEVTCL (Graphics & Canvas Engine)

The **UEVTCL** environment controls visual processing loops, coordinate tracking, and direct vector shapes.

### The Core Rendering Lifecycle
Applications run inside a continuous frame update loop executed via the native `BJVE.add()` listener:

```bjve
BJVE.add({
  draw(ctx) {
    ctx.fillStyle = "lime";
    ctx.fillRect(50, 50, 50, 50);
  }
});
```

### Native Canvas Context Commands:
* **`ctx.fillStyle = "[color_token]"`**: Configures the active color filling pattern. Accepts common language string tags (e.g., `"lime"`, `"black"`), hex matrices, or RGB parameters.
* **`ctx.fillRect(x, y, width, height)`**: Generates a solid 2D square or rectangle using the active styling pattern. The origin `(0,0)` rests firmly at the top-left boundaries of the window.
* **`ctx.clearRect(x, y, width, height)`**: Wipes canvas state pixel allocations clean within specified boundary parameters.

---

## 📐 3. OpenDraw Compilation Component

**OpenDraw** is a core sub-compiler operating within the UEVTCL graphic context. It intercepts raw `HTML(code)` layout strings and compiles them directly into native user interfaces without script overhead.

### The Transformation Formula
The conversion of static string markup into operational interface frames maps to the following pipeline:

$$\mathcal{R}(c) = \int \mathcal{P}(c) \cdot \mathcal{E}(\text{ctx}) \, dt$$

Where:
* **$c$**: The raw `HTML(code)` layout string input.
* **$\mathcal{P}(c)$**: The structural parser mapping node tags.
* **$\mathcal{E}(\text{ctx})$**: The execution bridge layer binding to the UEVTCL canvas.
* **$\mathcal{R}(c)$**: The final application state drawn inside the window viewport.

### Implementation Pattern:
```bjve
const appLayout = OpenDraw(HTML(`
  <div class="viewport-frame">
    <h1>Active System View</h1>
  </div>
`));

BJVE.add({
  layout: appLayout,
  draw(ctx) {
    // Graphic equations render concurrently here over the compiled layout
  }
});
```

---

## 🔥 4. Bjve Fire (Component State Engine)

The **Fire** variation handles global backend state tracking, logical loops, and dynamic instance handling.

### Instance Construction Mechanics
Objects and engine layout parts are allocated to active tracking memory blocks via internal class constructors using the `Instance.new` syntax blueprint:

```bjve
print("Hello Fire")

part = Instance.new("Part")
part.name = "Block"
part.position = {x = 10, y = 20}
```

### Strict Grammar Mapping:
* **Property Declaration**: Strings and names use standard text assignments (`part.name = "Block"`).
* **Coordinate Maps**: Coordinates and multi-dimensional positions **must** use explicit key-value tables (`{x = 10, y = 20}`) rather than Vector structures.

---

## 📑 5. Legacy Components & Deprecation Notes

### OpenCanvas (Obsolete)
* **Status**: Fully Deprecated.
* **Notice**: OpenCanvas managed early low-level pixel manipulation pipelines. All active projects must completely migrate legacy configurations over to the unified `OpenDraw(HTML(code))` matrix layout hook. 
