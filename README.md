# DebugTrace

DebugTrace is a C++ wrapper for DebugInfo DLL.

## Usage

### Step1

Copy ***DebugInfo.dll*** and ***DebugInfoX64.dll*** to your project folder where your executable file located. Based on the architecture of your project, you can copy only one dll, ***DebugInfo.dll*** for 32-bit architecture, ***DebugInfoX64.dll*** is a 64 bit architecture.

### Step2

Copy ***DebugTrace.cpp*** and ***DebugTrace.h*** to you project source folder and import them into your project through your compiler can build then.

### Step3

In your source where you need to print or log some message, change your code as one of below, then the message will present on the debug information form created by DebugInfo DLL.

```c++
#include "DebugTrace.h"
...
...
DEBUG_PRINT("your print message, and can using the format string such as: %d", number);
DEBUG_STRING("your log message as std::string, number = " + std::to_string(number));
```
