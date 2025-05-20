# 📚 Function Offset Documentation — Minecraft: Story Mode S1:CE

This file contains a curated list of functions identified in the binary, labeled by user-defined names and guessed roles based on reverse engineering.

> 💡 Offsets are relative to the main executable base.  
> 🏷️ Names are not official — they are inferred labels to aid documentation and discussion.

---

## 🗂 Function Table

| Offset     | Name                | Description / Guessed Purpose                                           |
|------------|---------------------|-------------------------------------------------------------------------|
| `0x1ECAC0` | `TT_LogShutdown`    | Called when shutting down a system; logs `.cpp` path for debug purposes |
| `0x1710` | `TT_StringReplaceSubstring`| Likely String insertion/replacement function                         |
| `0x1490` | `TT_StringReserveMemory` | Appears to be Memory allocation for string growth              |
| `0x16C00` | `TT_HeapFreeImpl` | Actual heap implementation function                        |
| `0x16980` | `TT_UpdateMemoryStats`   | Updates memory usage statistics                                  |
| `0x29D0`      | `TT_StringAppend`               | String append function                                                                     |
| `0x33C50`      | `TT_FreeStringMemory`               | Free string memory function                                                                     |
| `0x2770`      | `TT_InitEngineWithPath`               | Initialize engine with path                                                                     |
| `0x8F750`      | `TT_InitGameSystem`               | Initialize game subsystem                                                                     |
| `0x3720`      | `j_TT_InitGameSystem`               | Returns TT_InitGameSystem                                                                     |
| `0x159B10`      | `TT_ResetGameState`               | Reset game state                                                                     |
| `0x113650`      | `TT_ParseGameCommandLine`               | Parse game-specific command line                                                                     |
| `0x2860`      | `TT_LoadLuaScript`               | Load Lua script                                                                     |
| `0x133760`      | `TT_ShouldUseThreadedMode`               | Check if threaded mode should be used                                                                     |
| `0x1ECAC0`      | `TT_LogShutdown`               | Log shutdown message with file/line/subsystem being shutdown                                                                     |
| `0x3A660`      | `TT_DisplayShutdownMessage`               | Display engine shutdown message                                                                     |
| `0x1ED020`      | `TT_FinalizeShutdown`               | Finalize engine shutdown                                                                     |
| `0x1ECB90`      | `TT_CleanupResources`               | Cleanup engine resources                                                                     |
| `0xD290`      | `j_TT_CleanupResources`               | Returns TT_CleanupResources                                                                     |
| `0x8680`      | `TT_DestroyEngine`               | Destroy engine instance                                                                     |
| `0x1360`      | `TT_StringErase`               | String erasure function                                                                     |


---

## 📌 Notes

- When a function is renamed or better understood, update this table with more precise descriptions.
- Functions with unknown purpose should still be documented with `???` for offset/name/description as placeholders.
- You can link detailed disassembly or behavioral notes per-function in subfolders or `.txt` files later.

---

## 🔄 To Do

- Expand function list
- Cross-reference with Lua bindings
- Flag engine subsystems each function belongs to
