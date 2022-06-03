Run `npm i` then `npm repro` to reproduce vercel build error

```
Error! An unexpected error occurred in build: TypeError: Unable to require `.d.ts` file.
This is usually the result of a faulty configuration or import. Make sure there is a `.js`, `.json` or another executable extension and loader (attached before `ts-node`) available alongside `test.d.ts`.
    at getOutputTypeCheck (/Users/chang/projects/repros/vercel-build-dts-error/node_modules/@vercel/node/dist/index.js:104574:27)
    at compile (/Users/chang/projects/repros/vercel-build-dts-error/node_modules/@vercel/node/dist/index.js:104649:109)
    at compileTypeScript (/Users/chang/projects/repros/vercel-build-dts-error/node_modules/@vercel/node/dist/index.js:104059:31)
    at Job.readFile (/Users/chang/projects/repros/vercel-build-dts-error/node_modules/@vercel/node/dist/index.js:104085:30)
    at Job.emitDependency (/Users/chang/projects/repros/vercel-build-dts-error/node_modules/@vercel/node/dist/index.js:61748:39)
    at /Users/chang/projects/repros/vercel-build-dts-error/node_modules/@vercel/node/dist/index.js:61762:21
    at async Promise.all (index 0)
    at Job.emitDependency (/Users/chang/projects/repros/vercel-build-dts-error/node_modules/@vercel/node/dist/index.js:61757:9)
    at async Promise.all (index 0)
    at Object.nodeFileTrace (/Users/chang/projects/repros/vercel-build-dts-error/node_modules/@vercel/node/dist/index.js:61499:5)
    ```