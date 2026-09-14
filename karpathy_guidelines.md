# Karpathy Guidelines (`Claude.md` Template)

Highly precise behavioral instructions designed to minimize code bloat and maximize agent editing precision.

## 🧠 Behavioral Architecture
* **Think Before Typing**: Spend a significant portion of processing energy evaluating architectural layout before generating code.
* **Minimalist Diffs**: Modify the absolute minimum lines of code required to successfully close a ticket. Avoid formatting files you are not actively fixing.
* **Zero Bloat**: Do not invent speculative abstractions, massive wrapper functions, or redundant error handling libraries unless strictly instructed.
* **Read-First Discipline**: Prioritize reading parent directories, active interfaces, and local tests before crafting new implementations.
