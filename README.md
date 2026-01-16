<p align="center">
  
<h1 align="center">Notesnook</h1>
<h3 align="center">An end-to-end encrypted note taking alternative to Evernote.</h3>
<p align="center">
<a href="https://notesnook.com/">Website</a> | <a href="https://notesnook.com/about">About us</a> | <a href="https://notesnook.com/roadmap">Roadmap</a> | <a href="https://notesnook.com/downloads">Downloads</a> | <a href="https://twitter.com/@notesnook">Twitter</a> | <a href="https://discord.gg/5davZnhw3V">Discord</a>
</p>



### Technologies & languages

Notesnook is built using the following technologies:

1. JavaScript/Typescript — this repo is in a hybrid state. A lot of the newer code is being written in Typescript & the old code is slowly being ported over.
2. React — the whole front-end across all platforms is built using React.
3. React Native — For mobile apps we are using React Native
4. Electron — For desktop app
5. NPM — listed here because we **don't** use Yarn or PNPM or XYZ across any of our projects.

> **Note: Each project in the monorepo contains its own architecture details which you can refer to.**

### Monorepo structure

| Name                       | Path                                               | Description                                                          |
| -------------------------- | -------------------------------------------------- | -------------------------------------------------------------------- |
| `@notesnook/web`           | [/apps/web](/apps/web)                             | Web client                                                           |
| `@notesnook/desktop`       | [/apps/desktop](/apps/desktop)                     | Desktop client                                                       |
| `@notesnook/mobile`        | [/apps/mobile](/apps/mobile)                       | Android/iOS clients                                                  |
| `@notesnook/web-clipper`   | [/extensions/web-clipper](/extensions/web-clipper) | Web clipper                                                          |
| `@notesnook/core`          | [/packages/core](/packages/core)                   | Shared core between all platforms                                    |
| `@notesnook/crypto`        | [/packages/crypto](/packages/crypto)               | Cryptography library wrapper around libsodium                        |
| `@notesnook/clipper`       | [/packages/clipper](/packages/clipper)             | Web clipper core handling everything related to actual page clipping |
| `@notesnook/editor`        | [/packages/editor](/packages/editor)               | Notesnook editor + all extensions                                    |
| `@notesnook/editor-mobile` | [/packages/editor-mobile](/packages/editor-mobile) | A very thin wrapper around `@notesnook/editor` for mobile clients    |
| `@notesnook/logger`        | [/packages/logger](/packages/logger)               | Simple & pluggable logger                                            |
| `@notesnook/sodium`        | [/packages/sodium](/packages/sodium)               | Wrapper around libsodium to support Node.js & Browser                |
| `@notesnook/streamable-fs` | [/packages/streamable-fs](/packages/streamable-fs) | Streaming interface around an IndexedDB based file system            |
| `@notesnook/theme`         | [/packages/theme](/packages/theme)                 | The core 


