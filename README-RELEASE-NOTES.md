# CherryEssentials — release notes

This archive is a source handoff, not a compiled release. It preserves the prototype's existing implementation and updates its visible branding and plugin metadata. It must be completed and tested before production use.

## Build requirements
- JDK 25
- Gradle 8.14+ (or a compatible Gradle distribution)
- Network access to the PaperMC Maven repository

## Build
```bash
gradle clean build
```
The JAR, if the build succeeds, will be in `build/libs/`.

## Do not deploy yet
See `BUILD_STATUS.md`. The requested feature set is not complete, and no runtime test against Paper 26.3 has been performed.
