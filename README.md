# ghidra-stm32f0

This is a ghidra extension which is actually loader for the STM32F0 series of microcontrollers

## What it does
* Labels memory regions
* Labels IVT and entry point (assuming normal boot mode)

## Installation
You can install the loader via a zip on the releases page, or build the module yourself following instructions from the blog post

## Building
You just need Java, gradle and ghidra for building. Position in source dir and issue gradle command:

```
gradle -PGHIDRA_INSTALL_DIR=/opt/ghidra_9.1.2_PUBLIC
```

You can check what tasks you can also call with gradle with standard tasks options:

```
gradle tasks -PGHIDRA_INSTALL_DIR=/opt/ghidra_9.1.2_PUBLIC
```

Note: you can also put path to the ghidra in gradle.properties file:
```
GHIDRA_INSTALL_DIR=/opt/ghidra_9.1.2_PUBLIC
```

# Credits

stm32f0 ghidra loader extension is written by kost.

stm32f0 ghidra loader extension is based on @wrongbaud stm32f2 loader available here: https://github.com/wrongbaud/ghidra-stm32
(used initial commit: 6ca4f282d6aa678fe71e6c89c97ee1d4989a932f)

