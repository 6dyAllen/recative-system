# phonograph changelog

## 2.1.1

### Patch Changes

- 4551f19: fix: Suppress unexpected source ended event
- 2081c08: fix: Clip can be stuck when not playing

## 2.1.0

### Minor Changes

- abdf6c1: feat: Firefox compatibility by prepending ID3 header

### Patch Changes

- 0a44c3d: fix: Incorrect skipping of ID3 header

## 2.0.0

### Major Changes

- 15109d5: feat: Completely rewritten scheduling

### Minor Changes

- acbb9bf: feat: Add loop and fade feature

## 1.6.0

- Add a `clip.paused` property

## 1.5.1

- Clone audio data each time `chunk.createSource` is called, to allow playing previously-paused audio on Chrome ([#3](https://github.com/Rich-Harris/phonograph/issues/3))

## 1.5.0

- Port to TypeScript, add declarations

## 1.4.4

- Always clone data — fixes Chrome bug

## 1.4.2-3

- Prevent `clip.dispose()` from causing `clip.play()` promise rejection if called in `ended` handler

## 1.4.1

- Reject play promise on load/playback error

## 1.4.0

- Return a promise from `clip.play()`

## 1.3.7

- Handle non-200 responses

## 1.3.6

- Gah npm

## 1.3.5

- Always specify start time when starting a source

## 1.3.4

- Use `error.phonographCode` instead of `error.code`, to avoid writing to read-only properties

## 1.3.3

- Better error handling

## 1.3.2

- Don't error if content-length is missing

## 1.3.1

- Add `buffered` property

## 1.3.0

- Implement `clip.dispose()`
- Allow multiple load attempts
- Create new promise for each `buffer()` attempt
- Distinguish between `loaderror` and `playbackerror`

## 1.2.2

- Prevent infinite loop with short frame length
- Fire `error` events
- Linting

## 1.2.1

- Ensure progress event on load

## 1.2.0

- VBR support

## 1.1.8

- Rebuild before publishing, d'oh...

## 1.1.7

- Coerce `length`

## 1.1.6

- Init on iOS, and export `init` function

## 1.1.5

- Better logging
- Differentiate between `progress` and `loadprogress` events

## 1.1.4

- Fix `onready` check

## 1.1.3

- Remove logging

## 1.1.2

- Fix XHR loader and Safari decoding

## 1.1.1

- Prevent audible seams

## 1.1.0

- Implement `clip.clone()`

## 1.0.1

- Include files in `pkg.files`

## 1.0.0

- First release
