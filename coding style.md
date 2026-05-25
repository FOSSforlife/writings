# Self-Documenting Code Manifesto

- **Code should be as concise as it can be before becoming unreadable**.
- Code should describe what the app does and why.
  - Use docstrings anywhere you can.
  - **Optional:** write unit tests in the same file as source code (also known as in-source testing). Personally, this makes things easier for me by preserving context, especially in test-driven development. That said, I agree with [the advice from vitest](https://vitest.dev/guide/in-source.html#notes): "use separate test files instead for more complex tests like **components** or **E2E testing**."
- Whenever possible, code should be written as reusable modules that compose together in flexible ways. These can be deep modules or basic pure functions, depending on the context.
  - These modules should be rigorously tested and handle all edge cases, so that the developer composing them together can have fun and stay safe.
- There should be generally one correct way to do something, as defined in a style guide, community best practices, the standard library, or in the language itself.
  - This reduces decision fatigue when writing code, and reduces context switching when reading code.
- Transpilers often enable us to write the code in a language that aligns with human thinking (e.g. ClojureScript, TypeScript, Gleam), and have it output code that's widely compatible and understood by machines. Take advantage of this. Think of the code as an extension of your mind. Let the compiler do the heavy lifting.
