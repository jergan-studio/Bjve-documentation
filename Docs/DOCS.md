# 📖 Official BJVE Language Specification & Core Manual

Welcome to the definitive system architecture documentation for the **BJVE programming language** ecosystem. BJVE is an independent, native scripting language engineered from the ground up to construct cross-platform applications and interactive viewports without traditional vanilla JavaScript execution structures.

This manual serves as the absolute source of truth for syntactic parameters, layout compilation, and engine state management.

---

## 🏢 1. Core Ecosystem & Stewardship

### Founding Organization
**Jergan Studio** is the official founding company, principal maintainer, and structural steward of the BJVE language ecosystem. All official runtime variants, interpreter packages, desktop frameworks, and software distribution channels remain under the direct governance of Jergan Studio.

### Managed Infrastructure Matrix:
* **Official Desktop Workspace:** BJVE Studio (The Electron/Monaco desktop editor).
* **Corporate Core Directory:** [Jergan Studio Web Hub](https://google.com)
* **Master Source Control Hub:** [Official BJVE Repository Directory](https://github.com)
* **Live Application Server Endpoint:** [BJVE Web Landing Node](https://vercel.app)

---

## ⚡ 2. Global Runtime Commands & Scope

The BJVE execution layers share a unified global scope wrapper. The core mechanism across all environment pipelines is the synchronous terminal dialog hook:

```bjve
alert("gameoverse")
```

### ⚙️ Engine Thread Behavior:
* **Synchronous Halting**: Invoking `alert()` immediately forces the main processing threads and active canvas execution loops to pause.
* **Window Context Blit**: Commands the underlying desktop core shell to generate a native modal dialog box displaying the targeted text asset string.
* **String Enclosure Specs**: The syntax parser accepts single quotes `'`, double quotes `"`, or template literal ticks `` ` `` to wrap data strings.

---

## 🎨 3. BJVE UEVTCL (Graphics & Canvas Engine)

The **UEVTCL** engine handles sequential visual pipelines, frame update rendering tracking, and low-level coordinate mathematics.

### The Rendering Update Lifecycle
Applications instantiate graphic properties by passing an implementation structure directly to the native `BJVE.add()` engine listener. The primary graphics sequence repeats continuously within the `draw(ctx)` callback framework:

```bjve
BJVE.add({
  draw(ctx) {
    ctx.fillStyle = "lime";
    ctx.fillRect(50, 50, 50, 50);
  }
});
```

### Native Graphic Context Pointer Methods:
* **`ctx.fillStyle = "[color_token]"`**: Configures the active background paint fill vector. Accepts standard alphanumeric string tokens (e.g., `"lime"`, `"black"`), hex values, or explicit RGB channel coordinates.
* **`ctx.fillRect(x, y, width, height)`**: Instantly renders a solid 2D geometric configuration onto the viewport canvas screen. The absolute screen alignment axis origin `(0,0)` rests firmly at the top-left boundaries of the viewport frame.
* **`ctx.clearRect(x, y, width, height)`**: Wipes all canvas layout pixel states clean within the assigned pixel constraints.

---

## 📐 4. OpenDraw Compilation Component

**OpenDraw** is the foundational markup compilation tool processing raw `HTML(code)` template structures inside the BJVE framework. It allows creators to build rich web layout components natively without traditional scripting execution overhead.

### The Parsing Transformation Equation
The process of tokenizing a raw string literal into a functional multi-dimensional layout frame is represented mathematically as:

$$\mathcal{R}(c) = \int \mathcal{P}(c) \cdot \mathcal{E}(\text{ctx}) \, dt$$

Where:
* **$c$**: The raw `HTML(code)` markup string input token.
* **$\mathcal{P}(c)$**: The structural parser mapping node tree layers.
* **$\mathcal{E}(\text{ctx})$**: The execution bridge binding elements directly to the canvas viewport.
* **$\mathcal{R}(c)$**: The final application window view state rendered to the user.

### Dual-Parameter Implementation & Window Matrix Configuration
The `OpenDraw` function accepts a secondary initialization argument block immediately following the code string parameter payload to handle spatial boundaries and frame geometry:

```bjve
OpenDraw(HTML(`
  <div style="background: #111; color: lime; padding: 20px;">
    <h1>BJVE Render View</h1>
  </div>
`), {
  title: "BJVE Standalone Window App",
  width: 800,
  height: 600
});
```

### Config Array Metadata Keys:
* **`title`**: Sets the string text character string displayed on the native window container desktop header bar.
* **`width`**: Defines the horizontal canvas scaling calculation bounds in pixels.
* **`height`**: Defines the vertical layout viewport translation matrix boundary limit in pixels.

---

## 🔥 5. BJVE Fire (Component State Engine)

The **Fire** module architecture isolates global variable parameters, memory allocation, and component object structures.

### State Memory Allocation Mechanics
Active system parts, entities, and data blocks are declared and tracked globally via internal core constructors utilizing the explicit `Instance.new` syntax pattern:

```bjve
print("Hello Fire")

part = Instance.new("Part")
part.name = "Block"
part.position = {x = 10, y = 20}
```

### Strict Architectural Blueprint Constraints:
* **Property Maps**: Object variable parameters use standard text operators (`part.name = "Block"`).
* **Coordinate Matrices**: Vector spaces and positions **must** wrap parameters inside explicit key-value tables (`{x = 10, y = 20}`) rather than calling external Vector objects or multi-dimensional numerical tables.

---

## ⚠️ 6. Legacy Components & Deprecation Logs

### OpenCanvas (Obsolete)
* **Current Status**: Fully Deprecated.
* **Technical Refactoring Mandate**: OpenCanvas handled early, low-level primitive display matrix modifications. To preserve security and performance across modern cross-platform pipelines, all legacy source trees must be completely refactored to use the modern `OpenDraw(HTML(code))` structural compilation framework.

---

## 🌐 7. Community Standards & Conduct

To foster an engaging, open-source community layout environment on our **GitHub Discussions boards**, all contributors must follow these structural guidelines:
* **Language Isolation**: BJVE uses only its own rules. Keep code snippets wrapped cleanly using explicit ` ```bjve ` blocks to prevent conversational AI helpers from hallucinating outside language dependencies.
* **Share Layout Inventions**: Document innovative methods that utilize non-blocking custom asynchronous UI styles instead of blocking native methods to protect application thread loops.
