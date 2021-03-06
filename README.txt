Binary:
  Buffer Overflow:
  | Vulns:
  | | Typical buffer overflow
  | | Off-by-one
  | Protection:
  | | StackGuard/StackCookie/canary
  | | NX/DEP:
  | |   Bypass:
  | |     ROP
  | | Shadow Stack
  |   
  ASLR:
  | Bypass:
  | | Memory leak
  | | Relative addressing + Partial IP overwrite/Off-by-one overflow
  | | Weak randomization algorithm (BAD)
  | | Side channels
  | | Modules w/o ASLR:
  |     HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management\MoveImages:
  |     |  0 -> respect PE header's IMAGE_DLL_CHARACTERISTICS_DYNAMIC_BASE value
  |     | -1 -> ignores PE header's IMAGE_DLL_CHARACTERISTICS_DYNAMIC_BASE value and force randomize 
  CFG:
    Bypass (https://habr.com/ru/company/dsec/blog/305960/):
    | Turned off DEP tuns of CFG protection
    | Find CTF table and change/use
    | Modules withoud CFG
    | Unaligned functions
    | JIT-functions   
