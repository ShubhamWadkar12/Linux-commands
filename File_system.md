# Linux Filesystem Directory Structure

Linux follows a hierarchical filesystem structure that starts from the root directory (`/`). Every file and directory exists under this root directory.

## Linux Directory Structure

| Directory | Purpose | Remember It As |
|---|---|---|
| `/` | Entire filesystem starts here. | Root of everything |
| `/home` | Contains normal users' home directories. | Normal users' personal space |
| `/root` | Root administrator's home directory. | Administrator's personal space |
| `/etc` | Stores system-wide configuration files. | Configuration |
| `/var` | Stores logs and frequently changing data. | Variable data |
| `/tmp` | Stores temporary files. | Temporary storage |
| `/usr` | Contains applications, utilities, libraries, and shared resources. | User programs |
| `/opt` | Stores optional third-party software. | Optional software |
| `/boot` | Contains bootloader and kernel-related files. | Boot files |
| `/dev` | Contains device files representing hardware and virtual devices. | Devices |
| `/proc` | Provides process and kernel information through a virtual filesystem. | Process information |
| `/sys` | Provides information about the kernel, devices, and hardware. | System and device information |

## Important Points to Remember

- `/` is the starting point of the entire Linux filesystem.
- `/home` contains personal directories of normal users.
- `/root` is the home directory of the root administrator.
- `/etc` is important when troubleshooting configuration issues.
- `/var/log` is commonly used when investigating system and application logs.
- `/tmp` is used for temporary files.
- `/proc` and `/sys` are virtual filesystems that expose kernel and system information.

- Configuration files → `/etc`
- System logs → `/var/log`
- Normal user directories → `/home`
- Root administrator's home → `/root`
- Temporary files → `/tmp`
