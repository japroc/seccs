Binary:
  Buffer Overflow:
    Vulns:
      Typical buffer overflow
      Off-by-one
    Protection:
      StackGuard/StackCookie/canary
      NX/DEP
      Shadow Stack
ASLR
  Bypass:
    Memory leak
    Relative addressing + Partial IP overwrite
    Weak randomization algorithm (BAD)
    Side channels
    Modules w/o ASLR:
      HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management\MoveImages:
         0 -> respect PE header's IMAGE_DLL_CHARACTERISTICS_DYNAMIC_BASE value
        -1 -> ignores PE header's IMAGE_DLL_CHARACTERISTICS_DYNAMIC_BASE value and force randomize 
