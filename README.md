# Expo CLI Metro Bundler Random Crashes

This repository demonstrates a bug encountered with the Expo CLI Metro bundler where random crashes occur during development without providing helpful error messages. The crashes are inconsistent and interrupt the development workflow.

## Bug Description

The Expo Metro bundler would unexpectedly crash during development. No error messages or stack traces were provided in the terminal. The crashes occurred randomly, not tied to specific actions or code changes.  This issue disrupted the development process and required restarting the Expo development server.

## Reproduction Steps

Reproducing this bug proved difficult due to its inconsistent nature.  However, the provided `expoBug.js` simulates a similar environment to where the crash would occur within our project. This is mostly for demonstrating how the file structure looks like.

## Solution

The solution involved a combination of techniques. See the `expoBugSolution.js` file for code examples.   Further investigation is required to pinpoint the exact cause. 

- **Increased Memory:** Allocating more memory to the Expo development server sometimes helped reduce the frequency of crashes.
- **Clean Build:**  A clean build using `expo start --clear` or by clearing the cache directories sometimes resolved the issue temporarily.
- **Dependency Review:** Reviewing the project's dependencies for any known incompatibility with Expo or the Metro bundler could be necessary.  
- **Update Expo CLI and dependencies:**  Ensure the latest versions of Expo CLI and all project dependencies are installed to leverage any bug fixes related to bundler stability.