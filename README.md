# Expo CLI: Obscure Web Build Errors

This repository demonstrates a common yet elusive bug encountered when building Expo apps for web.  The issue arises from incompatibilities between native modules and the `react-native-web` environment.  While the error messages might be generic (like `Invariant Violation`), the root cause often lies in a seemingly innocuous dependency.

## Reproducing the Bug

The `bug.js` file contains a simplified example that mimics the problematic scenario.  By running `expo start --web`, you can observe the error.  The exact error message may vary.

## Solution

The `bugSolution.js` file provides a solution. The key is identifying the offending dependency and replacing it with a web-compatible alternative or by using conditional imports to load different modules based on the platform.