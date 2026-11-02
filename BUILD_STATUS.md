# CherryEssentials 1.0.0-dev — build status

This is a development source package based on the uploaded BerryEssentials prototype. Branding and plugin metadata have been changed to CherryEssentials.

**Important:** this package is NOT a production-ready release and does not contain all requested systems. In particular, Chest Shop, minimap adapters, NPC dialogs, full admin/member menus, Battlepass, full quest progression, and complete clan/rank integrations are not implemented. Existing prototype features also require additional testing and hardening.

Target: Paper 26.3 / Java 25. The build uses the Paper Maven repository and requires Gradle plus network access to resolve `paper-api`. No valid server-loadable JAR was built in the current environment because only Java 21 is installed, Gradle is absent, and external DNS/network access is unavailable.

Do not install this development source package as a JAR on a production server.
