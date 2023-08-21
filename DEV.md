# Develop Personal Web Page Using Hyde Template

---

## 1. Fast Reload 
- Make `jekyll serve` reflect changes immediately similar to react
- Download dependencies and run following commands
  - `npm install -g browser-sync`
  - create a `bs-config.js file` and add the following
    ```
    module.exports = {
      files: "_site/**/*", // Watch changes in the compiled site
      server: {
        baseDir: "_site", // Serve files from the compiled site
      },
    }
    ```
  - run `jekyll serve`  in a terminal
  - run `browser-sync start --config bs-config.js` in second terminal

