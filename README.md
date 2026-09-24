# Ntsec

ACN VB6 WinNT 4.0 security demo (`WinNtSecurity.exe`, project WinNtSecurity) that exercises Advapi32 ACL helpers in `modWinNTSecurity`. On load, `frmTest` calls `AddAccessControlElement` to GRANT COMMON_CHANGE on `c:\temp\test.txt` for a trustee, then `GetAccessControlElements` and prints each ACE trustee with resolved access mode/permissions. Module wraps `GetNamedSecurityInfo` / `SetNamedSecurityInfo`, `BuildExplicitAccessWithName`, and `SetEntriesInAcl` for file (and other SE_OBJECT_TYPE) DACLs.

**Source last updated:** 2026-08-27 · **Language:** VB6 · **Target:** VB6 Win32 · **Output:** WinForms exe

_Note: original OneDrive LastWriteTime values were wiped to 2026-08-27 by a zip transfer; date above uses best available evidence (headers/copyright where helpful)._

## Solution structure

| Project | Language | Type | Purpose |
|---------|----------|------|---------|
| `WinNtSecurity` (`WinNTSecurity.vbp`) | VB6 | WinForms exe | Demo add/list DACL ACEs on a named file object |

## How to open

Open the `.vbp` in Visual Basic 6.0 IDE:
- `WinNTSecurity.vbp`

## Requirements

- Visual Basic 6.0 IDE
- Windows Advapi32 privileges to read/write object security descriptors

## Attribution and provenance

Working copy from my Historical Dev folder `VB/Old/Ntsec`.
Company names in project files: ACN.
Project description: "Test the Windows Nt 4.0 Security".

## License

MIT (c) 2026 VaderConsulting for Dave Robinson's code. See `LICENSE`.
