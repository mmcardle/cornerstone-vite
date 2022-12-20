# cornerstone-vite

Example Vite app using Cornerstone3d 

# Status

Fails in dev with

```
CrosshairsTool.ts:54 Uncaught TypeError: Cannot read properties of undefined (reading 'vec2')
    at CrosshairsTool.ts:54:34
```

Fails in preview with

```
index-84a783b5.js:39643 Uncaught ReferenceError: Cannot access 'index' before initialization
    at index-84a783b5.js:39643:29
```

# Steps to create

    yarn create vite cornerstone-vite --template vue
    cd cornerstone-vite
    yarn add "@cornerstonejs/core" "@cornerstonejs/tools"
    yarn add "@kitware/vtk.js@25.9.0" "gl-matrix@^3.4.3"
    yarn add @types/d3-array@^3.0.3 @types/d3-interpolate@^3.0.1 d3-array@^3.0.3 d3-interpolate@^3.0.1

    yarn run dev

    yarn run build && yarn run 