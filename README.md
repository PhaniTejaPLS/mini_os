# 🧵 DIY OS Kernel in C++

## 📍 Goal
Build a basic OS kernel in C++ with:
- A bootloader
- Process/thread management
- A file system interface

---

## 📦 Phase 1: Environment Setup
- Install GCC cross-compiler (targeting `i386` or `x86_64`)
- Set up QEMU or Bochs for virtualization
- Create a `Makefile` for bootloader + kernel
- Prepare ISO image build script

---

## 📚 Learning Topics
- x86 architecture
- C++ in freestanding environments
- BIOS and UEFI basics
- Linkers, GRUB bootloader

---

## 🧠 Phase 2: Bootloader and Kernel Entry
- Write Stage 1 bootloader (Assembly)
- Use GRUB to load C++ kernel
- Create kernel entry function (`kernel_main`)
- Set up VGA text buffer output (custom `printf`)

---

## 🧠 Phase 3: Memory Management
- Paging and segmentation (implement basic page table)
- Kernel heap allocator (buddy allocator or slab allocator)
- Stack setup per process/thread

---

## ⚙️ Phase 4: Multitasking and Scheduling
- Implement Process Control Blocks (PCBs)
- Cooperative scheduling (round-robin)
- _Later:_ Pre-emptive scheduling with timer interrupts

---

## 📂 Phase 5: Filesystem Interface
- Implement virtual file system (VFS) layer
- Add ext2 or FAT32 support
- Add read/write syscalls

---

## ⛓️ Phase 6: Syscalls and User Mode
- Syscall table and interrupt handlers
- User-mode program loader
- IPC (pipes or message passing)

---

## 🧪 Testing and Debugging
- QEMU + GDB for step debugging
- Unit tests on memory allocator and scheduler
- Integration tests for file system operations
