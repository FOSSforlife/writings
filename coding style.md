# Self-Documenting Code Manifesto

- **Code should be as concise as it can be before becoming unreadable**.
- Code should describe what the app does and why.
- Whenever possible, code should be written as reusable **deep modules** that compose together in flexible ways.
  - These modules should be rigorously tested and handle all edge cases, so that the developer composing them together can have fun and stay safe.
- There should be generally one correct way to do something, as defined in a style guide, community best practices, the standard library, or in the language itself.
  - This reduces decision fatigue when writing code, and reduces context switching when reading code.
- Transpilers often enable us to write the code in a language that aligns with human thinking (e.g. ClojureScript, TypeScript, Gleam), and have it output code that's widely compatible and understood by machines. Take advantage of this. Think of the code as an extension of your mind. Let the compiler do the heavy lifting.
