- Optimization techniques :
  1. Minification
  2. Uglification
  3. Bundle
  4. Dead code elimination
  5. Ahead of time compilation

- For production production use.. ng build -prod
- Angular compiler take javascript code and produces javascript code. Angular compiler parse each component's template and resolve string inerpolation, event binding etc and creates corresponding javascript code at runtime.
- Compilation that happens at runtime is call Just in time(JIT) compilation, it works well during development phase.
- JIT compilation:
  - Inefficient for production
  - Happens for every user
  - More component more slower
  - We have to ship angular compiler with bundle

- Ahead of time compilation: Instead of compilation at runtime, user will download pre-compiled application.
  - Faster startup
  - No need to ship angular compiler with bundle
  - Catch template errors earlier.
  - Better security

- Package for angular compiler is - @angular/compiler-cli
- Angular compiler generates ngFactory file for every component.



