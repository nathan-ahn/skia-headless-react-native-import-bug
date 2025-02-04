# Reproduction Steps

1. Clone the repository.
2. `bun install --frozen-lockfile`
3. `bun ./src/index.ts`

# Results

Error: `Cannot find package 'react-native' from '.../skia-headless-react-native-import-bug/node_modules/@shopify/react-native-skia/lib/module/Platform/Platform.js'`

This bug was introduced in `v1.11.0` of `@shopify/react-native-skia`. You can test by swapping out the version for `v1.10.2` and see that running the reproduction steps does not error.
