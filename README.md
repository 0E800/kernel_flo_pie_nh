##3.4.113-Kali-0E800.nethunter-flo-1.0-g5452e51bb642

#Features:    
Android Security updates at March 5 2019   
Kernel patched for HID and Wifi Injection   


Build output:   
```

root@keys-daggers:~/kernel/google/msm# sh build.sh
Cleaning build...
Creating kernel config for nethunter-flo-1.0...
make: Entering directory '/root/rerpie/kernel/google/msm'
  HOSTCC  scripts/basic/fixdep
  GEN     /root/rerpie/kernel/google/msm/build/Makefile
  HOSTCC  scripts/kconfig/conf.o
  SHIPPED scripts/kconfig/zconf.tab.c
  SHIPPED scripts/kconfig/zconf.lex.c
  SHIPPED scripts/kconfig/zconf.hash.c
  HOSTCC  scripts/kconfig/zconf.tab.o
In file included from scripts/kconfig/zconf.tab.c:2500:
/root/rerpie/kernel/google/msm/scripts/kconfig/confdata.c: In function ‘conf_write’:
/root/rerpie/kernel/google/msm/scripts/kconfig/confdata.c:705:19: warning: ‘%s’ directive writing likely 7 or more bytes into a region of size between 1 and 4097 [-Wformat-overflow=]
  sprintf(newname, "%s%s", dirname, basename);
                   ^~~~~~
/root/rerpie/kernel/google/msm/scripts/kconfig/confdata.c:705:19: note: assuming directive output of 7 bytes
/root/rerpie/kernel/google/msm/scripts/kconfig/confdata.c:705:2: note: ‘sprintf’ output 1 or more bytes (assuming 4104) into a destination of size 4097
  sprintf(newname, "%s%s", dirname, basename);
  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/root/rerpie/kernel/google/msm/scripts/kconfig/confdata.c:708:20: warning: ‘.tmpconfig.’ directive writing 11 bytes into a region of size between 1 and 4097 [-Wformat-overflow=]
   sprintf(tmpname, "%s.tmpconfig.%d", dirname, (int)getpid());
                    ^~~~~~~~~~~~~~~~~
/root/rerpie/kernel/google/msm/scripts/kconfig/confdata.c:708:3: note: ‘sprintf’ output between 13 and 4119 bytes into a destination of size 4097
   sprintf(tmpname, "%s.tmpconfig.%d", dirname, (int)getpid());
   ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  HOSTLD  scripts/kconfig/conf
warning: (ARCH_MSM_KRAITMP && ARCH_MSM_CORTEX_A5) selects HAVE_HW_BRKPT_RESERVED_RW_ACCESS which has unmet direct dependencies (HAVE_HW_BREAKPOINT)
warning: (ARCH_MSM_KRAITMP && ARCH_MSM_CORTEX_A5) selects HAVE_HW_BRKPT_RESERVED_RW_ACCESS which has unmet direct dependencies (HAVE_HW_BREAKPOINT)
#
# configuration written to .config
#
make: Leaving directory '/root/rerpie/kernel/google/msm'
Starting build for nethunter-flo-1.0...
make: Entering directory '/root/rerpie/kernel/google/msm'
  GEN     /root/rerpie/kernel/google/msm/build/Makefile
scripts/kconfig/conf --silentoldconfig Kconfig
warning: (ARCH_MSM_KRAITMP && ARCH_MSM_CORTEX_A5) selects HAVE_HW_BRKPT_RESERVED_RW_ACCESS which has unmet direct dependencies (HAVE_HW_BREAKPOINT)
warning: (ARCH_MSM_KRAITMP && ARCH_MSM_CORTEX_A5) selects HAVE_HW_BRKPT_RESERVED_RW_ACCESS which has unmet direct dependencies (HAVE_HW_BREAKPOINT)
  GEN     /root/rerpie/kernel/google/msm/build/Makefile
  WRAP    arch/arm/include/generated/asm/auxvec.h
  WRAP    arch/arm/include/generated/asm/bitsperlong.h
  WRAP    arch/arm/include/generated/asm/cputime.h
  WRAP    arch/arm/include/generated/asm/emergency-restart.h
  WRAP    arch/arm/include/generated/asm/errno.h
  WRAP    arch/arm/include/generated/asm/ioctl.h
  WRAP    arch/arm/include/generated/asm/irq_regs.h
  WRAP    arch/arm/include/generated/asm/kdebug.h
  WRAP    arch/arm/include/generated/asm/local.h
  CHK     include/linux/version.h
  WRAP    arch/arm/include/generated/asm/local64.h
  WRAP    arch/arm/include/generated/asm/percpu.h
  WRAP    arch/arm/include/generated/asm/poll.h
  WRAP    arch/arm/include/generated/asm/resource.h
  UPD     include/linux/version.h
  WRAP    arch/arm/include/generated/asm/sections.h
  WRAP    arch/arm/include/generated/asm/siginfo.h
  WRAP    arch/arm/include/generated/asm/simd.h
  WRAP    arch/arm/include/generated/asm/sizes.h
  HOSTCC  scripts/kallsyms
  HOSTCC  scripts/conmakehash
  CC      scripts/mod/empty.o
  HOSTCC  scripts/genksyms/genksyms.o
  SHIPPED scripts/genksyms/lex.lex.c
  SHIPPED scripts/genksyms/keywords.hash.c
  SHIPPED scripts/genksyms/parse.tab.h
  SHIPPED scripts/genksyms/parse.tab.c
  HOSTCC  scripts/selinux/genheaders/genheaders
  HOSTCC  scripts/mod/mk_elfconfig
  HOSTCC  scripts/selinux/mdp/mdp
  HOSTCC  scripts/genksyms/parse.tab.o
  HOSTCC  scripts/bin2c
  MKELF   scripts/mod/elfconfig.h
  HOSTCC  scripts/mod/file2alias.o
  HOSTCC  scripts/mod/modpost.o
  HOSTCC  scripts/mod/sumversion.o
  HOSTCC  scripts/genksyms/lex.lex.o
  HOSTLD  scripts/mod/modpost
  HOSTLD  scripts/genksyms/genksyms
  Using /root/rerpie/kernel/google/msm as source for kernel
  CHK     include/generated/utsrelease.h
  UPD     include/generated/utsrelease.h
  Generating include/generated/mach-types.h
  CC      kernel/bounds.s
  GEN     include/generated/bounds.h
  CC      arch/arm/kernel/asm-offsets.s
  GEN     include/generated/asm-offsets.h
  CALL    /root/rerpie/kernel/google/msm/scripts/checksyscalls.sh
  CC      init/main.o
  CHK     include/generated/compile.h
  HOSTCC  usr/gen_init_cpio
  CC      init/do_mounts.o
  CC      init/do_mounts_rd.o
  CC      init/do_mounts_initrd.o
  CC      init/initramfs.o
  CC      init/calibrate.o
  CC      arch/arm/kernel/elf.o
  CC      arch/arm/vfp/vfpmodule.o
  AS      arch/arm/kernel/entry-armv.o
  AS      arch/arm/vfp/entry.o
  AS      arch/arm/kernel/entry-common.o
  AS      arch/arm/vfp/vfphw.o
  CC      arch/arm/mm/dma-mapping.o
  CC      arch/arm/kernel/irq.o
  CC      arch/arm/mm/extable.o
  CC      arch/arm/vfp/vfpsingle.o
  CC      arch/arm/kernel/opcodes.o
  CC      arch/arm/vfp/vfpdouble.o
  CC      arch/arm/kernel/process.o
  CC      arch/arm/mm/fault.o
  CC      arch/arm/common/gic.o
  LD      arch/arm/net/built-in.o
  CC      arch/arm/common/cpaccess.o
  PERL    arch/arm/crypto/aesbs-core.S_shipped
  UPD     include/generated/compile.h
  CC      arch/arm/crypto/aesbs-glue.o
  CC      init/version.o
In function ‘cpio_replace_env’,
    inlined from ‘cpio_mkfile_line’ at /root/rerpie/kernel/google/msm/usr/gen_init_cpio.c:454:26:
/root/rerpie/kernel/google/msm/usr/gen_init_cpio.c:399:4: warning: ‘strncpy’ output may be truncated copying 4096 bytes from a string of length 4096 [-Wstringop-truncation]
    strncpy(new_location, expanded, PATH_MAX);
    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  CC      arch/arm/mm/init.o
  CC      arch/arm/mm/iomap.o
  CC      arch/arm/kernel/ptrace.o
  CC      arch/arm/kernel/return_address.o
  CC      arch/arm/mm/fault-armv.o
  CC      arch/arm/mm/flush.o
  GEN     usr/initramfs_data.cpio
  AS      usr/initramfs_data.o
  CC      arch/arm/kernel/sched_clock.o
  CC      arch/arm/kernel/setup.o
  CC      arch/arm/kernel/signal.o
  LD      usr/built-in.o
  CC      arch/arm/kernel/stacktrace.o
  CC      arch/arm/perfmon/perf-function-hooks.o
  AS      arch/arm/crypto/aes-armv4.o
  CC      arch/arm/crypto/aes_glue.o
  CC      arch/arm/kernel/sys_arm.o
  CC      arch/arm/kernel/time.o
  CC      arch/arm/mach-msm/io.o
  CC      arch/arm/mm/idmap.o
  CC      arch/arm/mm/ioremap.o
  AS      arch/arm/crypto/sha1-armv7-neon.o
  CC      arch/arm/crypto/sha1_neon_glue.o
  CC      arch/arm/mm/mmap.o
  AS      arch/arm/crypto/sha1-armv4-large.o
  CC      arch/arm/kernel/traps.o
  CC      arch/arm/kernel/cpuidle.o
  CC      arch/arm/crypto/sha1_glue.o
  LD      arch/arm/common/built-in.o
  CC      arch/arm/kernel/armksyms.o
  CC      kernel/fork.o
  AS      arch/arm/crypto/sha512-armv7-neon.o
  LD      init/mounts.o
  CC      arch/arm/kernel/module.o
  CC      arch/arm/crypto/sha512_neon_glue.o
  LD      arch/arm/vfp/vfp.o
  LD      arch/arm/vfp/built-in.o
  CC      arch/arm/kernel/bios32.o
  CC      mm/filemap.o
  CC      arch/arm/kernel/isa.o
  CC      arch/arm/mm/pgd.o
  CC      arch/arm/mm/mmu.o
  SHIPPED arch/arm/crypto/aesbs-core.S
  AS      arch/arm/crypto/aesbs-core.o
  LD      init/built-in.o
  CC      arch/arm/mm/vmregion.o
  CC      arch/arm/mach-msm/dma.o
  AS      arch/arm/kernel/sleep.o
  CC      arch/arm/kernel/suspend.o
  CC      arch/arm/kernel/smp.o
  LD      arch/arm/perfmon/built-in.o
  CC      ipc/util.o
  CC      fs/open.o
  CC      ipc/msgutil.o
  CC      ipc/msg.o
  CC      arch/arm/mm/proc-syms.o
  CC      arch/arm/mm/alignment.o
  CC      arch/arm/kernel/smp_tlb.o
  CC      arch/arm/kernel/smp_scu.o
  CC      arch/arm/kernel/machine_kexec.o
  AS      arch/arm/kernel/relocate_kernel.o
  CC      arch/arm/kernel/atags.o
  CC      arch/arm/mm/highmem.o
  LD      arch/arm/crypto/aes-arm.o
  LD      arch/arm/crypto/aes-arm-bs.o
  CC      arch/arm/kernel/unwind.o
  LD      arch/arm/crypto/sha1-arm.o
  AS      arch/arm/mm/abort-ev7.o
  LD      arch/arm/crypto/sha1-arm-neon.o
  AS      arch/arm/mm/pabort-v7.o
  LD      arch/arm/crypto/sha512-arm-neon.o
  LD      arch/arm/crypto/built-in.o
  CC      arch/arm/kernel/swp_emulate.o
  CC      arch/arm/kernel/pmu.o
  CC      security/keys/gc.o
  CC      security/commoncap.o
  CC      crypto/api.o
  CC      security/min_addr.o
  AS      arch/arm/mm/cache-v7.o
  GEN     security/selinux/flask.h security/selinux/av_permissions.h
  CC      ipc/sem.o
  CC      security/selinux/avc.o
  CC      arch/arm/kernel/perf_event.o
  CC      arch/arm/mm/copypage-v6.o
  CC      arch/arm/mm/context.o
  CC      arch/arm/kernel/topology.o
  CC      arch/arm/kernel/io.o
  AS      arch/arm/kernel/head.o
  CC      ipc/shm.o
  AS      arch/arm/mm/tlb-v7.o
  CC      security/security.o
  CC      arch/arm/kernel/init_task.o
  CC      arch/arm/mach-msm/memory.o
  CC      ipc/ipcns_notifier.o
  CC      arch/arm/mach-msm/timer.o
  CC      security/keys/key.o
  CC      ipc/syscall.o
  LDS     arch/arm/kernel/vmlinux.lds
  CC      security/selinux/hooks.o
  CC      ipc/ipc_sysctl.o
  AS      arch/arm/mm/proc-v7.o
  CC      ipc/namespace.o
  CC      security/selinux/selinuxfs.o
  CC      security/selinux/netlink.o
  CC      security/selinux/nlmsgtab.o
  CC      block/elevator.o
  LD      arch/arm/mm/built-in.o
  CC      block/blk-core.o
  CC      block/blk-tag.o
  CC      sound/sound_core.o
  CC      fs/read_write.o
  LD      drivers/auxdisplay/built-in.o
  CC      drivers/base/core.o
  CC      block/blk-sysfs.o
  CC      drivers/base/bus.o
  CC      crypto/cipher.o
  CC      crypto/compress.o
  CC      crypto/algapi.o
  CC      security/selinux/netif.o
  CC      security/selinux/netnode.o
  CC      security/selinux/netport.o
  CC      arch/arm/mach-msm/clock.o
  CC      arch/arm/mach-msm/clock-voter.o
  LD      ipc/built-in.o
  LD      firmware/built-in.o
  CC      security/keys/keyring.o
  CC      security/selinux/exports.o
  CC      kernel/exec_domain.o
  CC      net/socket.o
  LD      sound/arm/built-in.o
  LD      sound/atmel/built-in.o
  CC      crypto/scatterwalk.o
  CC      mm/mempool.o
  LD      net/802/built-in.o
  CC      security/capability.o
  CC      arch/arm/mach-msm/clock-dummy.o
  CC      sound/core/compress_offload.o
  CC      net/bluetooth/af_bluetooth.o
  CC      sound/core/hwdep.o
  CC      block/blk-flush.o
  CC      security/selinux/ss/ebitmap.o
  CC      security/selinux/ss/hashtab.o
  CC      arch/arm/mach-msm/modem_notifier.o
  CC      security/selinux/ss/symtab.o
  LD      arch/arm/kernel/built-in.o
  CC      crypto/proc.o
  CC      security/selinux/ss/sidtab.o
  CC      arch/arm/mach-msm/subsystem_map.o
  CC      arch/arm/lib/uaccess_with_memcpy.o
  CC      drivers/base/dd.o
  AS      arch/arm/lib/ashldi3.o
  CC      kernel/panic.o
  CC      fs/file_table.o
  CC      security/selinux/ss/avtab.o
  AS      arch/arm/lib/ashrdi3.o
  CC      security/selinux/ss/policydb.o
  CC      drivers/base/syscore.o
  CC      security/keys/keyctl.o
  CC      crypto/ablkcipher.o
  CC      kernel/printk.o
  CC      mm/oom_kill.o
  CC      mm/fadvise.o
  CC      crypto/blkcipher.o
  CC      sound/core/memalloc.o
  AS      arch/arm/lib/backtrace.o
  CC      block/blk-settings.o
  CC      crypto/ahash.o
  CC      security/selinux/ss/services.o
  CC      sound/core/pcm.o
  AS      arch/arm/lib/call_with_stack.o
  CC      sound/core/pcm_native.o
  CC      drivers/base/driver.o
  AS      arch/arm/lib/changebit.o
  CC      security/selinux/ss/conditional.o
  CC      net/bluetooth/hci_core.o
  CC      kernel/cpu.o
  CC      arch/arm/mach-msm/cpufreq.o
  CC      security/lsm_audit.o
  CC      mm/maccess.o
  AS      arch/arm/lib/clear_user.o
  CC      fs/super.o
  CC      security/selinux/ss/mls.o
  AS      arch/arm/lib/clearbit.o
  AS      arch/arm/lib/csumipv6.o
  CC      security/keys/permission.o
  CC      drivers/base/class.o
  AS      arch/arm/lib/csumpartial.o
  CC      security/selinux/ss/status.o
  AS      arch/arm/lib/csumpartialcopy.o
  CC      sound/core/pcm_lib.o
  CC      mm/page_alloc.o
  CC      block/blk-ioc.o
  CC      net/caif/caif_dev.o
  CC      sound/core/pcm_timer.o
  CC      crypto/shash.o
  CC      crypto/algboss.o
  AS      arch/arm/lib/csumpartialcopyuser.o
  CC      arch/arm/lib/delay.o
  AS      arch/arm/lib/div64.o
  CC      arch/arm/mach-msm/nohlt.o
  AS      arch/arm/lib/findbit.o
  CC      kernel/exit.o
  CC      block/blk-map.o
  CC      security/keys/process_keys.o
  AS      arch/arm/lib/getuser.o
  CC      sound/core/pcm_misc.o
  CC      sound/core/pcm_memory.o
  AS      arch/arm/lib/io-readsb.o
  AS      arch/arm/lib/io-readsl.o
  AS      arch/arm/lib/io-readsw-armv4.o
  CC      arch/arm/mach-msm/clock-debug.o
  AS      arch/arm/lib/io-writesb.o
  CC      sound/core/rawmidi.o
  CC      kernel/itimer.o
  AS      arch/arm/lib/io-writesl.o
  AS      arch/arm/lib/io-writesw-armv4.o
  CC      drivers/base/platform.o
  AS      arch/arm/lib/lib1funcs.o
  AS      arch/arm/lib/lshrdi3.o
  AS      arch/arm/lib/memchr.o
  AS      arch/arm/lib/memset.o
  AS      arch/arm/lib/memzero.o
  AS      arch/arm/lib/muldi3.o
  CC      fs/char_dev.o
  CC      block/blk-exec.o
  AS      arch/arm/lib/putuser.o
  AS      arch/arm/lib/setbit.o
  CC      block/blk-merge.o
  CC      block/blk-softirq.o
  AS      arch/arm/lib/strchr.o
  CC      drivers/block/brd.o
  CC      drivers/block/loop.o
  CC      security/keys/request_key.o
  CC      drivers/block/zram/zcomp_lzo.o
  AS      arch/arm/lib/strncpy_from_user.o
  CC      drivers/block/zram/zcomp.o
  CC      arch/arm/mach-msm/msm_kexec.o
  CC      arch/arm/mach-msm/acpuclock.o
  CC      net/caif/cfcnfg.o
  AS      arch/arm/lib/strnlen_user.o
  CC      block/blk-timeout.o
  HZFILE  kernel/hz.bc
  CC      kernel/softirq.o
  CC      crypto/testmgr.o
  CC      sound/core/timer.o
  AS      arch/arm/lib/strrchr.o
  LD      security/selinux/selinux.o
  AS      arch/arm/lib/testchangebit.o
  LD      security/selinux/built-in.o
  AS      arch/arm/lib/testclearbit.o
  CC      arch/arm/mach-msm/acpuclock-krait.o
  AS      arch/arm/lib/testsetbit.o
  CC      arch/arm/mach-msm/msm-krait-l2-accessors.o
  AS      arch/arm/lib/ucmpdi2.o
  CC      fs/stat.o
  CC      drivers/bluetooth/hci_ldisc.o
  CC      drivers/base/cpu.o
  CC      block/blk-iopoll.o
  CC      drivers/block/zram/zram_drv.o
  LD      arch/arm/lib/built-in.o
  AR      arch/arm/lib/lib.a
  CC      security/keys/request_key_auth.o
  CC      fs/exec.o
  CC      security/keys/user_defined.o
  CC      net/caif/cfmuxl.o
  CC      lib/bcd.o
  CC      sound/core/sound.o
  CC      lib/div64.o
  CC      arch/arm/mach-msm/pmu.o
  CC      crypto/crypto_wq.o
  CC      fs/pipe.o
  CC      lib/sort.o
  CC      net/bluetooth/hci_conn.o
  CC      block/blk-lib.o
  CC      sound/core/init.o
  CC      security/keys/proc.o
  CC      kernel/resource.o
  CC      lib/parser.o
  CC      drivers/base/firmware.o
  CC      security/keys/sysctl.o
  CC      net/caif/cfctrl.o
  CC      block/ioctl.o
  CC      arch/arm/mach-msm/perf_event_msm_krait_l2.o
  CC      net/caif/cffrml.o
  CC      drivers/bluetooth/btusb.o
  CC      arch/arm/mach-msm/krait-scm.o
  CC      lib/halfmd4.o
  CC      fs/namei.o
  CC      fs/fcntl.o
  LD      crypto/crypto_algapi.o
  CC      sound/core/memory.o
  CC      sound/core/info.o
  CC      crypto/aead.o
  LD      security/keys/built-in.o
  LD      security/built-in.o
  CC      kernel/sysctl.o
  CC      drivers/base/init.o
  CC      drivers/base/map.o
  CC      lib/debug_locks.o
  CC      lib/random32.o
  CC      arch/arm/mach-msm/perf_debug.o
  CC      block/genhd.o
  CC      drivers/block/zram/zcomp_lz4.o
  CC      net/caif/cfveil.o
  CC      drivers/base/devres.o
  CC      lib/bust_spinlocks.o
  CC      sound/core/control.o
  AS      arch/arm/mach-msm/headsmp.o
  CC      sound/core/misc.o
  CC      sound/core/device.o
  CC      net/caif/cfdbgl.o
  CC      net/caif/cfserl.o
  CC      drivers/base/attribute_container.o
  CC      arch/arm/mach-msm/platsmp.o
  LD      drivers/block/zram/zram.o
  LD      drivers/block/zram/built-in.o
  LD      drivers/block/built-in.o
  CC      net/caif/cfdgml.o
  CC      lib/hexdump.o
  LD      drivers/cdrom/built-in.o
  CC      net/caif/cfrfml.o
  CC      kernel/sysctl_binary.o
  CC      mm/page-writeback.o
  CC      fs/ioctl.o
  CC      net/caif/cfvidl.o
  CC      block/scsi_ioctl.o
  CC      lib/kasprintf.o
  CC      net/caif/cfutill.o
  CC      net/caif/cfsrvl.o
  CC      fs/readdir.o
  CC      fs/select.o
  CC      arch/arm/mach-msm/hotplug.o
  CC      drivers/base/transport_class.o
  CC      lib/bitmap.o
  CC      net/caif/cfpkt_skbuff.o
  CC      sound/core/jack.o
  CC      net/caif/chnl_net.o
  CC      drivers/bluetooth/ath3k.o
  CC      lib/scatterlist.o
  CC      drivers/bluetooth/bluetooth-power.o
  CC      lib/string_helpers.o
  CC      net/caif/caif_socket.o
  LD      crypto/crypto_blkcipher.o
  CC      crypto/chainiv.o
  CC      crypto/eseqiv.o
  CC      arch/arm/mach-msm/avs.o
  CC      kernel/capability.o
  CC      drivers/base/topology.o
  CC [M]  drivers/bluetooth/bcm203x.o
  CC      net/bluetooth/hci_event.o
  CC [M]  drivers/bluetooth/bpa10x.o
  CC [M]  drivers/bluetooth/bfusb.o
  CC      fs/fifo.o
  CC      kernel/ptrace.o
  CC      block/partition-generic.o
  LD      crypto/crypto_hash.o
  CC      crypto/pcompress.o
  CC      drivers/base/sys.o
  CC      drivers/base/dma-contiguous.o
  LD      net/caif/caif.o
  CC      kernel/timer.o
  CC      kernel/user.o
  AS      arch/arm/mach-msm/idle-v7.o
  LD      sound/drivers/mpu401/built-in.o
  CC      lib/gcd.o
  LD      crypto/cryptomgr.o
  LD      sound/drivers/opl3/built-in.o
  LD      sound/drivers/opl4/built-in.o
  LD      sound/drivers/pcsp/built-in.o
  LD      sound/drivers/vx/built-in.o
  LD      sound/core/snd.o
  CC      drivers/char/mem.o
  LD      drivers/clocksource/built-in.o
  LD      sound/drivers/built-in.o
  CC      drivers/clk/clkdev.o
  CC      drivers/char/random.o
  LD      sound/core/snd-hwdep.o
  LD      sound/core/snd-timer.o
  CC      net/bluetooth/mgmt.o
  CC      drivers/char/misc.o
  LD      sound/core/snd-pcm.o
  CC      arch/arm/mach-msm/scm.o
  LD      sound/core/snd-page-alloc.o
  LD      sound/core/snd-rawmidi.o
  LD      sound/core/snd-compress.o
  LD      sound/core/built-in.o
  LD      sound/firewire/built-in.o
  LD      sound/i2c/other/built-in.o
  CC      fs/dcache.o
  LD      sound/i2c/built-in.o
  CC      lib/lcm.o
  LD      sound/isa/ad1816a/built-in.o
  LD      sound/isa/ad1848/built-in.o
  CC      kernel/signal.o
  LD      sound/isa/cs423x/built-in.o
  CC      kernel/sys.o
  CC      kernel/kmod.o
  LD      sound/isa/es1688/built-in.o
  LD      sound/isa/galaxy/built-in.o
  LD      net/caif/built-in.o
  LD      sound/isa/gus/built-in.o
  LD      sound/isa/msnd/built-in.o
  LD      sound/isa/opti9xx/built-in.o
  LD      sound/isa/sb/built-in.o
  LD      sound/isa/wavefront/built-in.o
  LD      drivers/bluetooth/hci_uart.o
  LD      sound/isa/wss/built-in.o
  LD      sound/isa/built-in.o
  CC      kernel/workqueue.o
  CC      drivers/cpufreq/cpufreq.o
  CC      drivers/base/power/sysfs.o
  CC      drivers/cpufreq/cpufreq_stats.o
  CC      lib/list_sort.o
  LD      sound/mips/built-in.o
  LD      sound/parisc/built-in.o
  CC      drivers/base/regmap/regmap.o
  LD      drivers/clk/built-in.o
  CC      crypto/hmac.o
  CC      mm/readahead.o
  CC      crypto/md4.o
  LD      drivers/bluetooth/built-in.o
  CC      drivers/base/regmap/regcache.o
  CC      arch/arm/mach-msm/scm-boot.o
  LD      sound/pci/ac97/built-in.o
  LD      sound/pci/ali5451/built-in.o
  CC      kernel/pid.o
  CC      drivers/base/regmap/regcache-rbtree.o
  LD      sound/pci/asihpi/built-in.o
  LD      sound/pci/au88x0/built-in.o
  LD      sound/pci/aw2/built-in.o
  LD      sound/pci/ca0106/built-in.o
  CC      drivers/char/diag/diagchar_core.o
  LD      sound/pci/cs46xx/built-in.o
  LD      sound/pci/cs5535audio/built-in.o
  CC      block/partitions/check.o
  LD      sound/pci/ctxfi/built-in.o
  LD      sound/pci/echoaudio/built-in.o
  CC      drivers/char/diag/diagchar_hdlc.o
  CC      lib/uuid.o
  LD      sound/pci/emu10k1/built-in.o
  LD      sound/pci/hda/built-in.o
  CC      arch/arm/mach-msm/peripheral-loader.o
  LD      sound/pci/ice1712/built-in.o
  LD      sound/pci/korg1212/built-in.o
  CC      block/partitions/msdos.o
  CC      drivers/base/power/generic_ops.o
  LD      sound/pci/lola/built-in.o
  CC      drivers/base/power/common.o
  LD      sound/pci/lx6464es/built-in.o
  CC      drivers/base/regmap/regcache-lzo.o
  LD      sound/pci/mixart/built-in.o
  CC      crypto/md5.o
  LD      sound/pci/nm256/built-in.o
  LD      sound/pci/oxygen/built-in.o
  LD      sound/pci/pcxhr/built-in.o
  CC      lib/flex_array.o
  LD      sound/pci/riptide/built-in.o
  CC      kernel/rcupdate.o
  LD      sound/pci/rme9652/built-in.o
  LD      sound/pci/trident/built-in.o
  CC      drivers/char/diag/diagfwd.o
  CC      drivers/base/regmap/regmap-debugfs.o
  LD      sound/pci/vx222/built-in.o
  LD      sound/pci/ymfpci/built-in.o
  LD      sound/pci/built-in.o
  CC      mm/swap.o
  CC      block/partitions/efi.o
  LD      sound/pcmcia/pdaudiocf/built-in.o
  CC      drivers/base/power/qos.o
  LD      sound/pcmcia/vx/built-in.o
  CC      drivers/base/power/main.o
  LD      sound/pcmcia/built-in.o
  CC      crypto/sha1_generic.o
  CC      crypto/sha256_generic.o
  CC      drivers/char/hw_random/core.o
  LD      sound/ppc/built-in.o
  LD      sound/sh/built-in.o
  CC      drivers/char/hw_random/msm_rng.o
  CC      lib/bsearch.o
  CC      sound/soc/soc-core.o
  CC      sound/soc/soc-dapm.o
  CC      drivers/base/regmap/regmap-i2c.o
  CC      lib/find_last_bit.o
  CC      drivers/cpufreq/cpufreq_performance.o
  CC      arch/arm/mach-msm/scm-pas.o
  CC      kernel/extable.o
  CC      kernel/params.o
  CC      kernel/posix-timers.o
  CC      drivers/base/regmap/regmap-spi.o
  CC      kernel/kthread.o
  CC      drivers/base/power/wakeup.o
  LD      block/partitions/built-in.o
  CC      block/bsg.o
  CC      lib/find_next_bit.o
  CC      crypto/sha512_generic.o
  CC      drivers/cpufreq/cpufreq_powersave.o
  CC      drivers/char/diag/diagmem.o
  LD      drivers/char/hw_random/rng-core.o
  LD      drivers/char/hw_random/built-in.o
  CC      fs/inode.o
  CC      drivers/char/msm_rotator.o
  CC      kernel/wait.o
  CC      lib/llist.o
  CC      lib/kstrtox.o
  CC      mm/truncate.o
  LD      drivers/base/regmap/built-in.o
  CC      drivers/cpufreq/cpufreq_userspace.o
  CC      drivers/base/dma-mapping.o
  CC      arch/arm/mach-msm/pil-q6v4.o
  CC      kernel/kfifo.o
  CC      drivers/char/diag/diagfwd_cntl.o
  CC      lib/pci_iomap.o
  CC      drivers/char/diag/diag_dci.o
  CC      lib/iomap_copy.o
  CC      kernel/sys_ni.o
  CC      net/bluetooth/hci_sock.o
  CC      kernel/posix-cpu-timers.o
  CC      drivers/base/power/runtime.o
  CC      lib/devres.o
  CC      kernel/mutex.o
  CC      lib/hweight.o
  CC      lib/bitrev.o
  CC      kernel/hrtimer.o
  CC      arch/arm/mach-msm/pil-riva.o
  CC      drivers/cpufreq/cpufreq_ondemand.o
  CC      crypto/ecb.o
  CC      drivers/base/dma-coherent.o
  CC      sound/soc/soc-jack.o
  CC      drivers/base/power/clock_ops.o
  CC      drivers/char/diag/diag_masks.o
  CC      lib/crc-ccitt.o
  CC      lib/crc16.o
  CC      block/noop-iosched.o
  HOSTCC  lib/gen_crc32table
  CC      arch/arm/mach-msm/pil-tzapps.o
  CC      kernel/rwsem.o
  CC      mm/vmscan.o
  CC      crypto/cbc.o
  CC      lib/libcrc32c.o
  CC      lib/genalloc.o
  CC      lib/lz4/lz4_compress.o
  CC      kernel/nsproxy.o
  CC      lib/lzo/lzo1x_compress.o
  CC      lib/lz4/lz4_decompress.o
  CC      lib/lzo/lzo1x_decompress_safe.o
  CC      arch/arm/mach-msm/pil-vidc.o
  CC      fs/attr.o
  CC      drivers/char/diag/diag_debugfs.o
  CC      net/bluetooth/hci_sysfs.o
  CC      block/deadline-iosched.o
  CC      kernel/srcu.o
  CC      kernel/semaphore.o
  CC      crypto/cryptd.o
  CC      lib/reed_solomon/reed_solomon.o
  LD      drivers/base/power/built-in.o
  CC      drivers/base/dma-buf.o
  CC      kernel/notifier.o
  CC      arch/arm/mach-msm/pil-dsps.o
  CC      sound/soc/soc-cache.o
  CC      sound/soc/soc-utils.o
  CC      arch/arm/mach-msm/pil-gss.o
  CC      drivers/cpufreq/cpufreq_interactive.o
  CC      drivers/cpufreq/freq_table.o
  CC      lib/zlib_deflate/deflate.o
  LD      lib/lzo/lzo_compress.o
  LD      lib/lzo/lzo_decompress.o
  LD      lib/lzo/built-in.o
  CC      drivers/char/diag/diagfwd_bridge.o
  CC      lib/zlib_deflate/deftree.o
  CC      lib/zlib_inflate/inffast.o
  LD      lib/lz4/built-in.o
  CC      net/bluetooth/l2cap_core.o
  CC      lib/textsearch.o
  CC      kernel/ksysfs.o
  CC      arch/arm/mach-msm/bam_dmux.o
  CC      fs/bad_inode.o
  CC      kernel/cred.o
  CC      block/cfq-iosched.o
  CC      kernel/async.o
  CC      kernel/range.o
  CC      arch/arm/mach-msm/smem_log.o
  CC      lib/zlib_inflate/inflate.o
  CC      arch/arm/mach-msm/ipc_logging.o
  CC      drivers/cpufreq/cpufreq_limit.o
  CC      drivers/base/firmware_class.o
  CC      kernel/groups.o
  CC      sound/soc/soc-pcm.o
  CC      sound/soc/soc-compress.o
  LD      lib/reed_solomon/built-in.o
  CC      fs/file.o
  LD      sound/sparc/built-in.o
  CC      drivers/char/diag/diagfwd_hsic.o
  CC      fs/filesystems.o
  CC      drivers/char/diag/diagfwd_smux.o
  CC      sound/soc/soc-io.o
  CC      kernel/lglock.o
  LD      sound/soc/atmel/built-in.o
  CC      net/bluetooth/l2cap_sock.o
  CC      crypto/des_generic.o
  CC      drivers/cpufreq/cpufreq_gov_msm.o
  LD      sound/soc/au1x/built-in.o
  LD      sound/soc/blackfin/built-in.o
  CC      kernel/smpboot.o
  CC      sound/soc/codecs/cs8427.o
  CC      lib/zlib_deflate/deflate_syms.o
  CC      sound/soc/codecs/msm_stub.o
  CC      kernel/events/core.o
  LD      drivers/char/diag/diagchar.o
  CC      kernel/events/ring_buffer.o
  LD      drivers/cpufreq/built-in.o
  CC      drivers/char/adsprpc.o
  CC      kernel/events/callchain.o
  CC      lib/zlib_inflate/infutil.o
  LD      sound/soc/davinci/built-in.o
  LD      sound/soc/ep93xx/built-in.o
  CC      net/core/sock.o
  LD      drivers/char/diag/built-in.o
  LD      sound/spi/built-in.o
  CC      net/core/request_sock.o
  LD      sound/synth/built-in.o
  CC      net/core/skbuff.o
  LD      lib/zlib_deflate/zlib_deflate.o
  LD      lib/zlib_deflate/built-in.o
  CC      lib/ts_kmp.o
  CC      lib/ts_bm.o
  CC      fs/namespace.o
  LD      sound/soc/fsl/built-in.o
  CC      fs/seq_file.o
  LD      sound/soc/imx/built-in.o
  CC      fs/xattr.o
  CC      kernel/irq/irqdesc.o
  CC      lib/zlib_inflate/inftrees.o
  CC      kernel/irq/handle.o
  CC      arch/arm/mach-msm/ipc_logging_debug.o
  CC      arch/arm/mach-msm/smd.o
  CC      arch/arm/mach-msm/smd_debug.o
  CC      lib/ts_fsm.o
  CC      sound/soc/codecs/wcd9304.o
  CC      drivers/base/module.o
  CC      lib/percpu_counter.o
  CC      crypto/twofish_generic.o
  CC      lib/zlib_inflate/inflate_syms.o
  CC      arch/arm/mach-msm/remote_spinlock.o
  CC      block/bfq-iosched.o
  CC      kernel/irq/manage.o
  LD      drivers/char/built-in.o
  CC      drivers/base/sync.o
  CC      drivers/base/sw_sync.o
  CC      mm/shmem.o
  CC      lib/audit.o
  CC      kernel/irq/spurious.o
  CC      net/core/iovec.o
  LD      lib/zlib_inflate/zlib_inflate.o
  LD      lib/zlib_inflate/built-in.o
  CC      lib/dynamic_debug.o
  CC      arch/arm/mach-msm/smd_private.o
  CC      net/bluetooth/smp.o
  CC      lib/nlattr.o
  CC      arch/arm/mach-msm/socinfo.o
  CC      fs/libfs.o
  CC      crypto/twofish_common.o
  CC      lib/average.o
  CC      arch/arm/mach-msm/hsic_tty.o
  CC      fs/fs-writeback.o
  CC      arch/arm/mach-msm/smd_tty.o
  CC      kernel/irq/resend.o
  CC      kernel/irq/chip.o
  CC      lib/cpu_rmap.o
  LD      sound/soc/jz4740/built-in.o
  CC      kernel/irq/dummychip.o
  LD      sound/soc/kirkwood/built-in.o
  LD      sound/soc/mid-x86/built-in.o
  CC      sound/soc/msm/qdsp6/q6asm.o
  CC      sound/soc/msm/qdsp6/q6adm.o
  CC      kernel/irq/devres.o
  CC      net/core/datagram.o
  CC      kernel/irq/autoprobe.o
  CC      arch/arm/mach-msm/smd_qmi.o
  CC      lib/dynamic_queue_limits.o
  CC      lib/argv_split.o
  CC      crypto/aes_generic.o
  CC      fs/pnode.o
  CC      arch/arm/mach-msm/smd_pkt.o
  CC      fs/drop_caches.o
  CC      net/core/stream.o
  CC      kernel/irq/irqdomain.o
  LD      drivers/base/built-in.o
  CC      net/bluetooth/sco.o
  CC      drivers/cpuidle/cpuidle.o
  CC      drivers/cpuidle/driver.o
  CC      drivers/cpuidle/governor.o
  CC      drivers/cpuidle/sysfs.o
  CC      lib/bug.o
  CC      lib/cmdline.o
  CC      fs/splice.o
  CC      fs/sync.o
  CC      net/core/scm.o
  CC      arch/arm/mach-msm/msm_dsps.o
  CC      drivers/cpuidle/governors/ladder.o
  CC      drivers/cpuidle/governors/menu.o
  CC      arch/arm/mach-msm/smd_nmea.o
  CC      mm/prio_tree.o
  CC      lib/cpumask.o
  CC      sound/soc/msm/qdsp6/q6afe.o
  CC      lib/ctype.o
  CC      lib/dec_and_lock.o
  CC      lib/decompress.o
  CC      lib/decompress_bunzip2.o
  CC      kernel/irq/proc.o
  CC      mm/util.o
  CC      sound/soc/msm/qdsp6/q6voice.o
  CC      lib/decompress_inflate.o
  LD      drivers/cpuidle/governors/built-in.o
  LD      drivers/cpuidle/built-in.o
  CC      crypto/arc4.o
  CC      crypto/deflate.o
  CC      net/core/gen_stats.o
  CC      crypto/michael_mic.o
  LD      drivers/crypto/built-in.o
  CC      arch/arm/mach-msm/reset_modem.o
  LD      drivers/firewire/built-in.o
  LD      drivers/firmware/built-in.o
  CC      crypto/crc32c.o
  CC      lib/decompress_unlzma.o
  CC      drivers/gpio/gpiolib.o
  CC      drivers/gpio/devres.o
  CC      sound/soc/codecs/wcd9304-tables.o
  CC      fs/utimes.o
  CC      crypto/authenc.o
  CC      lib/dump_stack.o
  CC      lib/extable.o
  CC      block/test-iosched.o
  CC      arch/arm/mach-msm/ipc_router_smd_xprt.o
  CC      arch/arm/mach-msm/ipc_router.o
  CC      arch/arm/mach-msm/ipc_socket.o
  CC      lib/idr.o
  CC      kernel/irq/pm.o
  CC      crypto/authencesn.o
  LD      kernel/events/built-in.o
  CC      crypto/rng.o
  CC      kernel/power/qos.o
  CC      kernel/power/main.o
  CC      net/core/gen_estimator.o
  CC      lib/int_sqrt.o
  CC      lib/ioremap.o
  CC      sound/soc/codecs/wcd9310.o
  CC      drivers/gpio/gpio-msm-common.o
  CC      sound/soc/codecs/wcd9310-tables.o
  CC      lib/irq_regs.o
  CC      net/core/net_namespace.o
  CC      crypto/krng.o
  LD      kernel/irq/built-in.o
  CC      fs/stack.o
  CC      kernel/sched/core.o
  CC      sound/soc/codecs/sound_control_gpl.o
  CC      crypto/ansi_cprng.o
  CC      crypto/ablk_helper.o
  CC      lib/is_single_threaded.o
  CC      mm/mmzone.o
  CC      kernel/power/console.o
  CC      lib/klist.o
  CC      lib/kobject.o
  CC      arch/arm/mach-msm/msm_ipc_router_security.o
  LD      crypto/crypto.o
  CC      arch/arm/mach-msm/smd_rpc_sym.o
  CC      arch/arm/mach-msm/asustek/devices_asustek.o
  CC      arch/arm/mach-msm/asustek/flo/board-flo.o
  CC      arch/arm/mach-msm/asustek/flo/board-flo-gpiomux.o
  CC      net/bluetooth/lib.o
  CC      fs/fs_struct.o
  CC      arch/arm/mach-msm/asustek/asustek-pcbid.o
  CC      lib/kobject_uevent.o
  LD      block/built-in.o
  CC      lib/md5.o
  CC      mm/vmstat.o
  CC      mm/backing-dev.o
  CC      net/core/secure_seq.o
  CC      kernel/power/process.o
  CC      sound/soc/codecs/sound_control_3_gpl.o
  CC      arch/arm/mach-msm/asustek/asustek-keypad.o
  CC      kernel/power/suspend.o
  LD      crypto/built-in.o
  CC      drivers/gpio/gpio-msm-v2.o
  AS      arch/arm/mach-msm/memutils/memcpy.o
  AS      arch/arm/mach-msm/memutils/copy_from_user.o
  CC      lib/memory_alloc.o
  CC      lib/plist.o
  CC      arch/arm/mach-msm/asustek/flo/board-flo-pmic.o
  AS      arch/arm/mach-msm/memutils/copy_to_user.o
  CC      arch/arm/mach-msm/memutils/copy_page.o
  CC      net/core/flow_dissector.o
  CC      drivers/gpio/pm8xxx-gpio.o
  CC      fs/statfs.o
  CC      fs/buffer.o
  CC      fs/bio.o
  CC      lib/prio_heap.o
  AS      arch/arm/mach-msm/memutils/memmove.o
  CC      net/dns_resolver/dns_key.o
  CC      drivers/gpio/pm8xxx-mpp.o
  CC      net/dns_resolver/dns_query.o
  LD      arch/arm/mach-msm/memutils/built-in.o
  CC      kernel/power/autosleep.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_core.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_fabric.o
  CC      net/bluetooth/amp.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_config.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_arb.o
  CC      lib/prio_tree.o
  CC      arch/arm/mach-msm/asustek/flo/board-flo-camera.o
  CC      arch/arm/mach-msm/asustek/flo/board-flo-gpu.o
  CC      lib/proportions.o
  LD      sound/soc/msm/qdsp6/built-in.o
  CC      lib/radix-tree.o
  CC      sound/soc/msm/msm-dai-q6-hdmi.o
  CC      sound/soc/msm/msm-pcm-voice.o
  CC      kernel/power/wakelock.o
  LD      net/dns_resolver/dns_resolver.o
  CC      kernel/power/poweroff.o
  LD      net/dns_resolver/built-in.o
  CC      net/ethernet/eth.o
  CC      mm/page_isolation.o
  CC      drivers/gpio/gpio-sx150x.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_bimc.o
  CC      fs/block_dev.o
  CC      fs/direct-io.o
  LD      sound/soc/mxs/built-in.o
  CC      lib/ratelimit.o
  LD      sound/soc/nuc900/built-in.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_noc.o
  CC      lib/rbtree.o
  CC      arch/arm/mach-msm/asustek/flo/board-flo-regulator.o
  CC      arch/arm/mach-msm/asustek/flo/board-flo-display.o
  CC      kernel/power/wakeup_reason.o
  CC      arch/arm/mach-msm/qdsp6v2/apr.o
  CC      net/core/sysctl_net_core.o
  CC      net/core/dev.o
  CC      mm/mm_init.o
  CC      lib/reciprocal_div.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_of.o
  CC      sound/soc/msm/msm-pcm-voip.o
  CC      lib/rwsem-spinlock.o
  CC      arch/arm/mach-msm/asustek/flo/board-flo-storage.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_rpm.o
  LD      drivers/gpio/built-in.o
  CC      lib/sha1.o
  LD      drivers/gpu/drm/i2c/built-in.o
  LD      drivers/gpu/drm/built-in.o
  CC      drivers/gpu/ion/ion.o
  CC      lib/show_mem.o
  CC      drivers/gpu/ion/ion_heap.o
  CC      fs/mpage.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_board_8960.o
  LD      kernel/power/built-in.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_board_8064.o
  CC      mm/mmu_context.o
  CC      lib/string.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_board_8930.o
  CC      arch/arm/mach-msm/msm_bus/msm_bus_dbg.o
  CC      net/core/ethtool.o
  CC      lib/timerqueue.o
  CC      drivers/gpu/ion/ion_system_heap.o
  LD      arch/arm/mach-msm/asustek/flo/built-in.o
  LD      net/ethernet/built-in.o
  LD      arch/arm/mach-msm/asustek/built-in.o
  CC      arch/arm/mach-msm/pm-boot.o
  CC      net/core/dev_addr_lists.o
  CC      net/ipv4/route.o
  CC      arch/arm/mach-msm/qdsp6v2/apr_v1.o
  CC      arch/arm/mach-msm/qdsp6v2/apr_tal.o
  CC      lib/vsprintf.o
  CC [M]  lib/crc-itu-t.o
  CC      mm/percpu.o
  CC      kernel/time/timekeeping.o
  CC      kernel/time/ntp.o
  CC      kernel/time/clocksource.o
  GEN     lib/crc32table.h
  CC      arch/arm/mach-msm/pm-8x60.o
  CC      lib/crc32.o
  CC      sound/soc/msm/msm-pcm-hostless.o
  CC      drivers/gpu/msm/adreno_ringbuffer.o
  CC      arch/arm/mach-msm/qdsp6v2/q6core.o
  LD      net/bluetooth/bluetooth.o
  CC      arch/arm/mach-msm/qdsp6v2/dsp_debug.o
  CC      drivers/gpu/ion/ion_carveout_heap.o
  LD      net/bluetooth/built-in.o
  CC      kernel/trace/trace_clock.o
  CC      kernel/trace/ring_buffer.o
  CC      fs/ioprio.o
  CC      net/ipv6/af_inet6.o
  CC      net/ipv6/anycast.o
  CC      sound/soc/msm/msm8960.o
  LD      arch/arm/mach-msm/msm_bus/built-in.o
  CC      arch/arm/mach-msm/pm-data.o
  CC      arch/arm/mach-msm/pm-stats.o
  CC      kernel/time/jiffies.o
  CC      net/core/dst.o
  CC      fs/proc_namespace.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_acdb.o
  CC      kernel/trace/trace.o
  CC      drivers/gpu/ion/ion_iommu_heap.o
  CC      drivers/gpu/ion/ion_cp_heap.o
  LD      lib/built-in.o
  CC      drivers/gpu/ion/ion_cma_heap.o
  CC      arch/arm/mach-msm/qdsp6v2/aac_in.o
  LD      sound/soc/codecs/snd-soc-wcd9304.o
  LD      sound/soc/codecs/snd-soc-wcd9310.o
  LD      sound/soc/codecs/snd-soc-cs8427.o
  LD      sound/soc/codecs/snd-soc-msm-stub.o
  LD      sound/soc/codecs/built-in.o
  CC      drivers/gpu/msm/adreno_drawctxt.o
  LD      sound/soc/omap/built-in.o
  CC      drivers/gpu/msm/adreno_dispatch.o
  CC      kernel/time/timer_list.o
  CC      arch/arm/mach-msm/pcie.o
  CC      net/core/netevent.o
  CC      kernel/time/timecompare.o
  CC      fs/cifs/cifsfs.o
  CC      fs/cifs/cifssmb.o
  CC      net/ipv6/ip6_output.o
  CC      fs/configfs/inode.o
  CC      fs/configfs/file.o
  CC      mm/compaction.o
  CC      arch/arm/mach-msm/qdsp6v2/qcelp_in.o
  CC      drivers/gpu/ion/msm/msm_ion.o
  AR      lib/lib.a
  CC      drivers/gpu/ion/msm/ion_cp_common.o
  CC      arch/arm/mach-msm/qdsp6v2/evrc_in.o
  CC      sound/soc/msm/apq8064.o
  CC      kernel/time/timeconv.o
  CC      kernel/time/posix-clock.o
  CC      kernel/time/alarmtimer.o
  CC      kernel/time/clockevents.o
  CC      net/core/neighbour.o
  CC      fs/configfs/dir.o
  CC      fs/configfs/symlink.o
  CC      drivers/gpu/msm/adreno_postmortem.o
  CC      kernel/sched/clock.o
  CC      arch/arm/mach-msm/pcie_irq.o
  CC      net/ipv6/ip6_input.o
  CC      net/core/rtnetlink.o
  CC      arch/arm/mach-msm/qdsp6v2/amrnb_in.o
  CC      kernel/time/tick-common.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_utils.o
  LD      drivers/gpu/ion/msm/built-in.o
  LD      drivers/gpu/ion/built-in.o
  CC      fs/cifs/cifs_debug.o
  CC      arch/arm/mach-msm/spm-v2.o
  CC      kernel/trace/trace_output.o
  LD      drivers/gpu/stub/built-in.o
  CC      fs/configfs/mount.o
  CC      kernel/time/tick-broadcast.o
  CC      kernel/sched/idle_task.o
  CC      drivers/gpu/msm/adreno_snapshot.o
  CC      drivers/gpu/vga/vgaarb.o
  CC      net/ipv4/inetpeer.o
  CC      mm/fremap.o
  CC      kernel/time/tick-oneshot.o
  CC      kernel/time/tick-sched.o
  CC      mm/highmem.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_wma.o
  CC      kernel/sched/fair.o
  CC      arch/arm/mach-msm/spm_devices.o
  CC      fs/configfs/item.o
  CC      arch/arm/mach-msm/dma_test.o
  CC      net/ipv6/addrconf.o
  CC      sound/soc/msm/msm8930.o
  CC      sound/soc/msm/mpq8064.o
  CC      net/ipv6/addrlabel.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_wmapro.o
  CC      mm/madvise.o
  CC      net/core/utils.o
  CC      fs/cifs/connect.o
  CC      drivers/gpu/msm/adreno_coresight.o
  CC      drivers/gpu/msm/adreno_trace.o
  CC      fs/cifs/dir.o
  LD      fs/configfs/configfs.o
  LD      fs/configfs/built-in.o
  CC      fs/debugfs/inode.o
  CC      fs/debugfs/file.o
  CC      arch/arm/mach-msm/rpm-regulator.o
  LD      kernel/time/built-in.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_aac.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_multi_aac.o
  CC      mm/memory.o
  CC      mm/mincore.o
  CC      drivers/gpu/msm/adreno_a2xx.o
  CC      drivers/gpu/msm/adreno_a2xx_trace.o
  CC      kernel/trace/trace_stat.o
  CC      net/ipv4/protocol.o
  LD      drivers/gpu/vga/built-in.o
  CC      drivers/gpu/msm/adreno_a2xx_snapshot.o
  CC      net/ipv6/route.o
  CC      net/ipv6/ip6_fib.o
  CC      net/ipv6/ipv6_sockglue.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_utils_aio.o
  CC      net/core/link_watch.o
  CC      arch/arm/mach-msm/qdsp6v2/rtac.o
  CC      sound/soc/msm/apq8064-i2s.o
  CC      mm/mlock.o
  CC      net/core/filter.o
  CC      drivers/gpu/msm/adreno_a3xx.o
  CC      drivers/gpu/msm/adreno_a4xx.o
  CC      fs/cifs/inode.o
  CC      fs/cifs/file.o
  CC      kernel/trace/trace_printk.o
  LD      fs/debugfs/debugfs.o
  LD      fs/debugfs/built-in.o
  CC      fs/devpts/inode.o
  CC      net/core/sock_diag.o
  CC      net/core/flow.o
  CC      net/ipv4/ip_input.o
  CC      sound/soc/msm/msm-dai-q6.o
  CC      drivers/gpu/msm/adreno_a3xx_trace.o
  CC      drivers/gpu/msm/adreno_a3xx_snapshot.o
  LD      fs/devpts/devpts.o
  LD      fs/devpts/built-in.o
  LD      fs/exofs/built-in.o
  CC      fs/ext2/balloc.o
  CC      kernel/sched/rt.o
  CC      kernel/sched/stop_task.o
  CC      kernel/trace/trace_sched_switch.o
  CC      arch/arm/mach-msm/qdsp6v2/q6audio_v1.o
  CC      mm/mmap.o
  CC      fs/cifs/link.o
  CC      arch/arm/mach-msm/rpm-regulator-8960.o
  CC      arch/arm/mach-msm/qdsp6v2/q6audio_v1_aio.o
  CC      net/ipv6/ndisc.o
  CC      drivers/gpu/msm/adreno.o
  CC      net/core/net-sysfs.o
  CC      net/core/fib_rules.o
  CC      kernel/sched/sched_avg.o
  CC      net/core/net-traces.o
  CC      net/ipv4/ip_fragment.o
  CC      net/ipv6/udp.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_mp3.o
  CC      drivers/gpu/msm/adreno_cp_parser.o
  CC      fs/cifs/misc.o
  CC      kernel/trace/trace_nop.o
  CC      arch/arm/mach-msm/rpm-regulator-8930.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_amrnb.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_amrwb.o
  CC      fs/ext2/dir.o
  CC      sound/soc/msm/msm-pcm-q6.o
  CC      fs/ext2/file.o
  CC      fs/cifs/netmisc.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_amrwbplus.o
  CC      fs/cifs/smbencrypt.o
  CC      kernel/trace/blktrace.o
  CC      arch/arm/mach-msm/subsystem_notif.o
  CC      net/ipv6/udplite.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_evrc.o
  CC      kernel/sched/cpupri.o
  CC      arch/arm/mach-msm/qdsp6v2/audio_qcelp.o
  CC      arch/arm/mach-msm/qdsp6v2/amrwb_in.o
  CC      fs/ext2/ialloc.o
  CC      net/ipv6/raw.o
  CC      arch/arm/mach-msm/qdsp6v2/adsp-loader.o
  CC      drivers/gpu/msm/adreno_debugfs.o
  CC      fs/cifs/transport.o
  CC      fs/ext2/inode.o
  CC      kernel/trace/trace_events.o
  LD      kernel/sched/built-in.o
  CC      kernel/trace/trace_export.o
  CC      kernel/freezer.o
  CC      sound/usb/card.o
  CC      arch/arm/mach-msm/qdsp6v2/ultrasound/q6usm.o
  CC      arch/arm/mach-msm/subsystem_restart.o
  CC      arch/arm/mach-msm/qdsp6v2/ultrasound/usf.o
  CC      fs/cifs/asn1.o
  CC      mm/mprotect.o
  CC      mm/mremap.o
  CC      fs/cifs/cifs_unicode.o
  CC      net/ipv4/ip_forward.o
  CC      sound/soc/msm/msm-multi-ch-pcm-q6.o
  CC      net/ipv6/protocol.o
  CC      net/ipv6/icmp.o
  CC      net/ipv6/mcast.o
  CC      drivers/gpu/msm/kgsl.o
  CC      drivers/gpu/msm/kgsl_trace.o
  LD      net/core/built-in.o
  CC      fs/ext2/ioctl.o
  CC      net/key/af_key.o
  CC      net/ipv6/reassembly.o
  CC      kernel/trace/trace_event_perf.o
  CC      mm/msync.o
  CC      kernel/profile.o
  CC      mm/rmap.o
  CC      fs/ext2/namei.o
  CC      sound/usb/clock.o
  CC      fs/cifs/nterr.o
  CC      fs/cifs/xattr.o
  CC      fs/cifs/cifsencrypt.o
  CC      net/ipv4/ip_options.o
  CC      net/ipv6/tcp_ipv6.o
  CC      arch/arm/mach-msm/ramdump.o
  CC      fs/ext2/super.o
  CC      arch/arm/mach-msm/qdsp6v2/ultrasound/usfcdev.o
  CC      net/ipv6/ping.o
  CC      fs/ext2/symlink.o
  CC      mm/vmalloc.o
  CC      fs/cifs/readdir.o
  CC      sound/soc/msm/msm-lowlatency-pcm-q6.o
  CC      kernel/trace/trace_events_filter.o
  CC      sound/usb/endpoint.o
  CC      kernel/trace/power-traces.o
  CC      fs/ext2/xattr.o
  CC      fs/ext2/xattr_user.o
  CC      net/ipv6/exthdrs.o
  CC      arch/arm/mach-msm/sysmon.o
  LD      arch/arm/mach-msm/qdsp6v2/ultrasound/built-in.o
  LD      arch/arm/mach-msm/qdsp6v2/built-in.o
  CC      fs/cifs/ioctl.o
  CC      net/ipv6/datagram.o
  CC      fs/cifs/sess.o
  CC      fs/ext2/xattr_trusted.o
  CC      kernel/stacktrace.o
  CC      arch/arm/mach-msm/modem-8960.o
  CC      net/ipv6/ip6_flowlabel.o
  CC      net/ipv6/inet6_connection_sock.o
  CC      fs/cifs/export.o
  CC      mm/pagewalk.o
  CC      net/ipv6/sysctl_net_ipv6.o
  CC      net/ipv6/xfrm6_policy.o
  CC      sound/soc/msm/msm-pcm-routing.o
  CC      net/ipv6/xfrm6_state.o
  CC      sound/usb/format.o
  CC      kernel/futex.o
  LD      fs/ext2/ext2.o
  LD      fs/ext2/built-in.o
  CC      fs/ext3/balloc.o
  CC      net/ipv4/ip_output.o
  CC      net/ipv4/ip_sockglue.o
  CC      net/ipv6/xfrm6_input.o
  CC      arch/arm/mach-msm/lpass-8960.o
  CC      drivers/gpu/msm/kgsl_sharedmem.o
  CC      arch/arm/mach-msm/wcnss-ssr-8960.o
  CC      mm/pgtable-generic.o
  CC      mm/process_vm_access.o
  CC      net/ipv6/xfrm6_output.o
  LD      net/key/built-in.o
  CC      net/l2tp/l2tp_core.o
  CC      net/ipv6/netfilter.o
  CC      arch/arm/mach-msm/gss-8064.o
  LD      fs/cifs/cifs.o
  CC      kernel/trace/rpm-traces.o
  LD      fs/cifs/built-in.o
  CC      sound/usb/helper.o
  CC      net/ipv6/fib6_rules.o
  CC      arch/arm/mach-msm/cpuidle.o
  CC      net/l2tp/l2tp_ppp.o
  CC      fs/ext4/balloc.o
  CC      net/ipv6/proc.o
  CC      net/ipv6/ah6.o
  CC      mm/init-mm.o
  CC      net/ipv6/esp6.o
  CC      arch/arm/mach-msm/msm_watchdog.o
  CC      mm/bootmem.o
  CC      net/ipv6/ipcomp6.o
  CC      sound/usb/mixer.o
  CC      sound/usb/mixer_quirks.o
  AS      arch/arm/mach-msm/msm_watchdog_asm.o
  CC      mm/memblock.o
  CC      drivers/gpu/msm/kgsl_pwrctrl.o
  CC      arch/arm/mach-msm/clock-local.o
  CC      net/ipv6/xfrm6_tunnel.o
  CC      sound/soc/msm/msm-dai-fe.o
  CC      sound/soc/msm/msm-compr-q6.o
  CC      net/ipv6/tunnel6.o
  LD      kernel/trace/built-in.o
  CC      fs/ext3/bitmap.o
  CC      net/ipv6/xfrm6_mode_transport.o
  CC      drivers/gpu/msm/kgsl_pwrscale.o
  CC      kernel/rtmutex.o
  CC      net/ipv6/xfrm6_mode_tunnel.o
  CC      arch/arm/mach-msm/clock-dss-8960.o
  CC      net/ipv6/xfrm6_mode_beet.o
  CC      fs/ext4/bitmap.o
  CC      net/ipv6/mip6.o
  CC      sound/soc/msm/msm-dai-stub.o
  CC      sound/usb/pcm.o
  CC      net/ipv6/netfilter/ip6_tables.o
  CC      mm/bounce.o
  CC      net/ipv4/inet_hashtables.o
  CC      net/ipv6/sit.o
  CC      arch/arm/mach-msm/clock-8960.o
  CC      mm/page_io.o
  CC      arch/arm/mach-msm/clock-rpm.o
  CC      fs/ext3/dir.o
  CC      fs/ext3/file.o
  CC      fs/ext4/dir.o
  CC      net/ipv6/addrconf_core.o
  CC      net/ipv4/inet_timewait_sock.o
  LD      net/l2tp/built-in.o
  CC      sound/soc/msm/msm-pcm-lpa.o
  CC      net/ipv6/exthdrs_core.o
  CC      kernel/smp.o
  CC      kernel/spinlock.o
  CC      fs/f2fs/dir.o
  CC      mm/swap_state.o
  LD      sound/soc/pxa/built-in.o
  LD      sound/soc/s6000/built-in.o
  LD      net/mac80211/built-in.o
  CC [M]  net/mac80211/main.o
  CC      net/ipv6/output_core.o
  CC [M]  net/mac80211/status.o
  CC      sound/usb/proc.o
  CC      net/ipv6/inet6_hashtables.o
  LD      net/ipv6/ipv6.o
  CC      fs/ext3/fsync.o
  CC      sound/usb/quirks.o
  CC      fs/ext3/ialloc.o
  CC      fs/ext3/inode.o
  CC      fs/ext3/ioctl.o
  CC      sound/soc/msm/msm-pcm-afe.o
  CC      kernel/uid16.o
  CC      fs/ext4/file.o
  CC      sound/usb/stream.o
  CC      drivers/gpu/msm/kgsl_mmu.o
  CC      mm/swapfile.o
  CC      kernel/module.o
  CC      fs/ext3/namei.o
  CC      fs/ext3/super.o
  CC      fs/ext3/symlink.o
  CC      sound/soc/msm/asustek_headset.o
  CC      fs/ext3/hash.o
  CC      arch/arm/mach-msm/clock-pll.o
  CC      net/ipv4/inet_connection_sock.o
  CC      sound/usb/midi.o
  CC      net/ipv4/tcp.o
  CC      fs/ext3/resize.o
  CC      net/ipv6/netfilter/ip6table_filter.o
  CC      fs/f2fs/file.o
  CC      fs/ext3/ext3_jbd.o
  CC      net/ipv4/tcp_input.o
  CC      kernel/kallsyms.o
  CC      fs/ext4/fsync.o
  LD      sound/soc/msm/snd-soc-qdsp6.o
  LD      sound/soc/msm/snd-soc-msm8960.o
  LD      sound/soc/msm/snd-soc-hostless-pcm.o
  LD      sound/usb/6fire/built-in.o
  CC      fs/ext3/xattr.o
  CC      fs/ext3/xattr_user.o
  LD      sound/usb/caiaq/built-in.o
  CC [M]  net/mac80211/sta_info.o
  LD      sound/usb/misc/built-in.o
  CC      arch/arm/mach-msm/footswitch-8x60.o
  LD      sound/usb/usx2y/built-in.o
  CC      fs/ext3/xattr_trusted.o
  CC      arch/arm/mach-msm/acpuclock-8960.o
  CC      arch/arm/mach-msm/acpuclock-8960ab.o
  CC      arch/arm/mach-msm/memory_topology.o
  LD      sound/soc/msm/built-in.o
  CC [M]  net/mac80211/wep.o
  CC      net/ipv6/netfilter/ip6table_mangle.o
  LD      sound/soc/samsung/built-in.o
  LD      sound/soc/sh/built-in.o
  LD      sound/soc/tegra/built-in.o
  LD      sound/soc/txx9/built-in.o
  LD      sound/soc/snd-soc-core.o
  LD      sound/soc/built-in.o
  CC      net/ipv6/netfilter/ip6table_raw.o
  CC      fs/ext4/ialloc.o
  CC      fs/ext4/inode.o
  CC      arch/arm/mach-msm/saw-regulator.o
  CC      fs/ext4/page-io.o
  CC      arch/arm/mach-msm/devices-8960.o
  CC      drivers/gpu/msm/kgsl_gpummu.o
  CC      arch/arm/mach-msm/devices-8064.o
  CC      kernel/kexec.o
  CC      kernel/cgroup.o
  CC      arch/arm/mach-msm/acpuclock-8064.o
  CC      arch/arm/mach-msm/acpuclock-8930.o
  CC      net/ipv4/tcp_output.o
  CC      mm/thrash.o
  CC      mm/dmapool.o
  CC      arch/arm/mach-msm/acpuclock-8627.o
  CC      net/ipv6/netfilter/ip6table_nat.o
  CC [M]  net/mac80211/wpa.o
  CC      net/ipv6/netfilter/nf_conntrack_l3proto_ipv6.o
  CC      net/ipv6/netfilter/nf_conntrack_proto_icmpv6.o
  CC      arch/arm/mach-msm/acpuclock-8930aa.o
  CC      arch/arm/mach-msm/acpuclock-8930ab.o
  CC      arch/arm/mach-msm/rpm.o
  LD      sound/usb/snd-usb-audio.o
  CC      fs/ext4/ioctl.o
  LD      sound/usb/snd-usbmidi-lib.o
  LD      sound/usb/built-in.o
  CC      sound/last.o
  CC      arch/arm/mach-msm/rpm_resources.o
  CC      drivers/gpu/msm/kgsl_iommu.o
  CC      arch/arm/mach-msm/mpm.o
  CC      mm/sparse.o
  CC      arch/arm/mach-msm/rpm_stats.o
  CC      arch/arm/mach-msm/rpm_master_stat.o
  CC      fs/f2fs/inode.o
  LD      sound/soundcore.o
  LD      sound/built-in.o
  CC      fs/ext4/namei.o
  CC      mm/ksm.o
  CC      kernel/cgroup_freezer.o
  CC      fs/ext4/super.o
  CC      net/ipv6/netfilter/nf_defrag_ipv6_hooks.o
  CC      net/ipv6/netfilter/nf_conntrack_reasm.o
  CC      net/ipv6/netfilter/nf_nat_l3proto_ipv6.o
  CC [M]  net/mac80211/scan.o
  CC      fs/ext4/symlink.o
  CC      arch/arm/mach-msm/rpm_rbcpr_stats.o
  GZIP    kernel/config_data.gz
  CC      kernel/res_counter.o
  CC [M]  net/mac80211/offchannel.o
  CC      arch/arm/mach-msm/rpm_log.o
  CC      arch/arm/mach-msm/tz_log.o
  CC      arch/arm/mach-msm/msm_xo.o
  CC      arch/arm/mach-msm/msm-buspm-dev.o
  CC      kernel/stop_machine.o
  CC      mm/slub.o
  CC      fs/ext4/hash.o
  CC      net/ipv4/tcp_timer.o
  CC      fs/f2fs/namei.o
  CC      net/ipv4/tcp_ipv4.o
  CC      arch/arm/mach-msm/devices-iommu.o
  CC      arch/arm/mach-msm/iommu_domains.o
  CC      arch/arm/mach-msm/event_timer.o
  CC      arch/arm/mach-msm/gpiomux-v2.o
  CC      net/ipv6/netfilter/nf_nat_proto_icmpv6.o
  CC      net/ipv6/netfilter/ip6t_rpfilter.o
  CC      arch/arm/mach-msm/gpiomux.o
  LD      fs/ext3/ext3.o
  CC      drivers/gpu/msm/kgsl_snapshot.o
  LD      fs/ext3/built-in.o
  CC      arch/arm/mach-msm/msm_dcvs_scm.o
  CC      mm/migrate.o
  CC      fs/ext4/resize.o
  CC      fs/fat/cache.o
  CC      arch/arm/mach-msm/msm_dcvs.o
  CC      fs/ext4/extents.o
  CC      net/ipv6/netfilter/ip6t_REJECT.o
  CC      arch/arm/mach-msm/msm_mpdecision.o
  CC [M]  net/mac80211/ht.o
  CC      net/ipv4/tcp_minisocks.o
  LD      net/ipv6/netfilter/nf_conntrack_ipv6.o
  LD      net/ipv6/netfilter/nf_defrag_ipv6.o
  LD      net/ipv6/netfilter/nf_nat_ipv6.o
  CC      net/ipv4/tcp_cong.o
  CC      arch/arm/mach-msm/msm_rq_stats.o
  CC      arch/arm/mach-msm/msm_show_resume_irq.o
  CC      fs/f2fs/hash.o
  CC      fs/ext4/ext4_jbd2.o
  CC      fs/fat/dir.o
  CC      drivers/hid/hid-lg.o
  CC      drivers/hid/hid-debug.o
  CC      kernel/audit.o
  CC      fs/ext4/migrate.o
  CC      drivers/hid/hid-core.o
  CC      net/ipv4/datagram.o
  CC      arch/arm/mach-msm/restart.o
  LD      net/ipv6/netfilter/built-in.o
  CC      net/ipv4/raw.o
  LD      net/ipv6/built-in.o
  CC      net/netfilter/core.o
  CC      fs/f2fs/super.o
  CC      net/netfilter/nf_log.o
  CC      drivers/gpu/msm/kgsl_events.o
  CC      fs/ext4/mballoc.o
  CC      drivers/gpu/msm/kgsl_debugfs.o
  CC      mm/cleancache.o
  CC [M]  net/mac80211/agg-tx.o
  CC      fs/ext4/block_validity.o
  CC      fs/ext4/move_extent.o
  CC      arch/arm/mach-msm/mdm2.o
  CC      drivers/hid/hid-input.o
  CC      net/ipv4/udp.o
  CC      arch/arm/mach-msm/mdm_common.o
  CC      arch/arm/mach-msm/cache_erp.o
  CC      net/ipv4/udplite.o
  CC      net/ipv4/arp.o
  CC      net/ipv4/icmp.o
  CC      mm/zsmalloc.o
  CC      drivers/gpu/msm/kgsl_pwrscale_trustzone.o
  CC      fs/ext4/mmp.o
  CC      net/netfilter/nf_queue.o
  CC      fs/fat/fatent.o
  CC      arch/arm/mach-msm/ebi_erp.o
  CC      arch/arm/mach-msm/msm_cache_dump.o
  CC      net/netfilter/nf_sockopt.o
  CC      drivers/hid/hidraw.o
  CC      drivers/gpu/msm/kgsl_sync.o
  CC      kernel/auditfilter.o
  CC      net/ipv4/devinet.o
  CC      arch/arm/mach-msm/hsic_sysmon.o
  CC      fs/ext4/indirect.o
  CC      arch/arm/mach-msm/fastchg.o
  CC      fs/ext4/xattr.o
  CC      arch/arm/mach-msm/msm_cpu_pwrctl.o
  CC      net/ipv4/af_inet.o
  CC      net/ipv4/igmp.o
  CC [M]  net/mac80211/agg-rx.o
  CC [M]  net/mac80211/ibss.o
  CC      drivers/gpu/msm/z180.o
  CC      drivers/gpu/msm/z180_postmortem.o
  CC      drivers/gpu/msm/z180_trace.o
  CC      fs/ext4/xattr_user.o
  CC      net/netfilter/nf_conntrack_core.o
  LD      mm/built-in.o
  CC      net/netfilter/nf_conntrack_standalone.o
  CC      net/netfilter/nf_conntrack_expect.o
  CC      fs/fat/file.o
  CC      drivers/hid/uhid.o
  LD      arch/arm/mach-msm/built-in.o
  CC      drivers/hid/hid-a4tech.o
  CC      drivers/hid/hid-axff.o
  CC      net/ipv4/fib_frontend.o
  CC      net/ipv4/fib_semantics.o
  CC      drivers/hid/hid-apple.o
  CC      fs/ext4/xattr_trusted.o
  CC      fs/ext4/xattr_security.o
  CC      kernel/auditsc.o
  LD      drivers/gpu/msm/msm_kgsl_core.o
  LD      drivers/gpu/msm/msm_adreno.o
  LD      drivers/gpu/msm/msm_z180.o
  CC      drivers/hid/hid-belkin.o
  LD      drivers/gpu/msm/built-in.o
  LD      drivers/gpu/built-in.o
  CC      drivers/hid/hid-cherry.o
  CC      drivers/hid/hid-chicony.o
  CC      drivers/hid/hid-cypress.o
  LD      drivers/hsi/clients/built-in.o
  CC      drivers/hid/hid-dr.o
  LD      drivers/hsi/built-in.o
  CC      drivers/hwmon/hwmon.o
  CC      drivers/hid/hid-emsff.o
  CC      net/netfilter/nf_conntrack_helper.o
  CC      drivers/hwmon/pm8xxx-adc.o
  CC [M]  net/mac80211/work.o
  CC      net/ipv4/fib_trie.o
  CC [M]  net/mac80211/iface.o
  CC      drivers/hid/hid-ezkey.o
  CC      fs/fat/inode.o
  CC      drivers/hid/hid-gyration.o
  CC      net/ipv4/inet_fragment.o
  CC      net/netfilter/nf_conntrack_proto.o
  CC      drivers/hid/hid-holtekff.o
  CC      fs/f2fs/inline.o
  CC      drivers/hid/hid-kensington.o
  CC      drivers/hid/hid-keytouch.o
  CC      net/netfilter/nf_conntrack_l3proto_generic.o
  CC      drivers/hid/hid-kye.o
  CC      drivers/hid/hid-lcpower.o
  CC      drivers/hwmon/pm8xxx-adc-scale.o
  CC      net/ipv4/ping.o
  CC      net/ipv4/sysctl_net_ipv4.o
  LD      drivers/hid/hid-logitech.o
  CC      drivers/hid/hid-logitech-dj.o
  CC      drivers/hid/hid-microsoft.o
  CC      drivers/hid/hid-monterey.o
  CC      drivers/hid/hid-multitouch.o
  CC      drivers/hid/hid-ntrig.o
  CC      drivers/hid/hid-ortek.o
  CC [M]  net/mac80211/rate.o
  CC      drivers/hid/hid-prodikeys.o
  CC      net/ipv4/sysfs_net_ipv4.o
  CC      net/ipv4/proc.o
  CC      net/ipv4/fib_rules.o
  CC      drivers/hid/hid-pl.o
  CC      net/netfilter/nf_conntrack_proto_generic.o
  CC      drivers/hwmon/epm_adc.o
  CC      net/netfilter/nf_conntrack_proto_tcp.o
  CC      drivers/hwmon/cap1106.o
  CC      fs/f2fs/checkpoint.o
  CC      net/netfilter/nf_conntrack_proto_udp.o
  CC      drivers/hid/hid-petalynx.o
  CC      net/ipv4/esp4.o
  CC      drivers/hid/hid-picolcd.o
  CC      net/netfilter/nf_conntrack_extend.o
  CC      drivers/hid/hid-primax.o
  CC      kernel/audit_watch.o
  CC      drivers/hid/hid-roccat.o
  CC      drivers/hid/hid-roccat-common.o
  CC      net/netfilter/nf_conntrack_acct.o
  CC      fs/fat/misc.o
  CC      drivers/hid/hid-roccat-arvo.o
  CC      net/ipv4/tunnel4.o
  CC      net/ipv4/xfrm4_mode_transport.o
  CC      drivers/hid/hid-roccat-isku.o
  CC [M]  net/mac80211/michael.o
  CC [M]  net/mac80211/tkip.o
  CC      drivers/hid/hid-roccat-kone.o
  LD      fs/ext4/ext4.o
  LD      fs/ext4/built-in.o
  CC      drivers/hid/hid-roccat-koneplus.o
  CC [M]  net/mac80211/aes_ccm.o
  CC      net/ipv4/xfrm4_mode_tunnel.o
  CC [M]  net/mac80211/aes_cmac.o
  CC      net/ipv4/ipconfig.o
  CC      net/ipv4/netfilter.o
  CC      net/ipv4/netfilter/nf_conntrack_l3proto_ipv4_compat.o
  CC      drivers/hid/hid-roccat-kovaplus.o
  CC      kernel/audit_tree.o
  CC      net/ipv4/netfilter/nf_conntrack_l3proto_ipv4.o
  LD      drivers/hwmon/built-in.o
  CC      net/netfilter/nf_conntrack_ecache.o
  CC      net/netfilter/nf_conntrack_labels.o
  CC      net/ipv4/inet_diag.o
  CC      fs/fat/namei_vfat.o
  CC      net/netfilter/nf_conntrack_h323_main.o
  CC      net/ipv4/tcp_diag.o
  CC      net/netfilter/nf_conntrack_h323_asn1.o
  CC      net/netfilter/nf_nat_core.o
  CC      drivers/hid/hid-roccat-pyra.o
  CC      drivers/hid/hid-saitek.o
  CC      drivers/hid/hid-samsung.o
  CC      fs/f2fs/gc.o
  CC [M]  net/mac80211/cfg.o
  CC      drivers/hid/hid-sjoy.o
  CC      net/ipv4/udp_diag.o
  CC [M]  net/mac80211/rx.o
  CC [M]  net/mac80211/spectmgmt.o
  CC      net/ipv4/tcp_cubic.o
  CC      drivers/hid/hid-sony.o
  CC      net/ipv4/netfilter/nf_conntrack_proto_icmp.o
  CC      drivers/hid/hid-speedlink.o
  CC      net/netfilter/nf_nat_proto_unknown.o
  CC [M]  net/mac80211/tx.o
  CC [M]  net/mac80211/key.o
  CC      drivers/hid/hid-sunplus.o
  CC      drivers/hid/hid-gaff.o
  CC      drivers/hid/hid-tmff.o
  CC      net/ipv4/netfilter/nf_nat_l3proto_ipv4.o
  CC      kernel/seccomp.o
  CC      net/ipv4/xfrm4_policy.o
  CC      drivers/hid/hid-tivo.o
  CC      drivers/hid/hid-topseed.o
  CC      net/ipv4/netfilter/nf_nat_proto_icmp.o
  CC      drivers/hid/hid-twinhan.o
  LD      fs/fat/fat.o
  LD      fs/fat/vfat.o
  LD      fs/fat/built-in.o
  CC [M]  net/mac80211/util.o
  CC      fs/fuse/dev.o
  CC      net/ipv4/xfrm4_state.o
  CC      net/ipv4/xfrm4_input.o
  CC      drivers/hid/hid-uclogic.o
  CC      net/netfilter/nf_nat_proto_common.o
  CC      drivers/hid/hid-zpff.o
  CC      drivers/hid/hid-zydacron.o
  CC      net/ipv4/netfilter/nf_defrag_ipv4.o
  CC      drivers/hid/hid-waltop.o
  CC      net/ipv4/xfrm4_output.o
  CC      drivers/hid/usbhid/hid-core.o
  LD      drivers/hid/hid.o
  CC      drivers/hid/usbhid/hid-quirks.o
  CC      net/ipv4/netfilter/nf_nat_h323.o
  CC      kernel/rcutree.o
  CC      net/ipv4/netfilter/nf_nat_pptp.o
  CC      net/ipv4/netfilter/nf_nat_proto_gre.o
  CC      net/netfilter/nf_nat_proto_udp.o
  CC      net/netfilter/nf_nat_proto_tcp.o
  CC      net/netfilter/nf_nat_helper.o
  CC      fs/f2fs/data.o
  CC      fs/f2fs/node.o
  CC      net/netfilter/nfnetlink_queue_core.o
  CC      net/netfilter/nfnetlink_queue_ct.o
  CC      net/netfilter/nfnetlink.o
  CC      net/ipv4/netfilter/ip_tables.o
  CC      net/ipv4/netfilter/iptable_filter.o
  CC      net/netfilter/nfnetlink_log.o
  CC [M]  net/mac80211/wme.o
  CC      net/netfilter/nf_conntrack_proto_dccp.o
  CC      net/netfilter/nf_conntrack_proto_gre.o
  CC      net/netfilter/nf_conntrack_proto_sctp.o
  CC [M]  net/mac80211/event.o
  CC      net/ipv4/netfilter/iptable_mangle.o
  CC      net/ipv4/netfilter/iptable_nat.o
  CC      net/netfilter/nf_conntrack_proto_udplite.o
  CC      net/netfilter/nf_conntrack_netlink.o
  CC      net/ipv4/netfilter/iptable_raw.o
  CC      net/ipv4/netfilter/iptable_security.o
  CC      net/ipv4/netfilter/ipt_ah.o
  CC      net/netfilter/nfnetlink_cthelper.o
  CC [M]  net/mac80211/chan.o
  CC [M]  net/mac80211/driver-trace.o
  CC [M]  net/mac80211/mlme.o
  CC      kernel/utsname_sysctl.o
  CC [M]  net/mac80211/led.o
  CC      fs/fuse/dir.o
  CC      net/ipv4/netfilter/ipt_rpfilter.o
  CC      net/ipv4/netfilter/ipt_MASQUERADE.o
  LD      drivers/hid/usbhid/usbhid.o
  LD      drivers/hid/usbhid/built-in.o
  LD      drivers/hid/built-in.o
  CC      net/netfilter/nf_conntrack_amanda.o
  CC      net/netfilter/nf_conntrack_ftp.o
  LD      net/netfilter/nf_conntrack_h323.o
  CC      net/ipv4/netfilter/ipt_NETMAP.o
  CC      net/ipv4/netfilter/ipt_REDIRECT.o
  CC      net/ipv4/netfilter/ipt_REJECT.o
  CC      drivers/i2c/i2c-boardinfo.o
  CC      drivers/i2c/i2c-core.o
  CC      kernel/tracepoint.o
  CC      kernel/elfcore.o
  CC      kernel/irq_work.o
  CC      net/netfilter/nf_conntrack_irc.o
  CC      net/netfilter/nf_conntrack_broadcast.o
  CC      kernel/cpu_pm.o
  CC [M]  net/mac80211/pm.o
  BC      kernel/timeconst.h
  CHK     kernel/config_data.h
  UPD     kernel/config_data.h
  CC      kernel/time.o
  CC      net/ipv4/netfilter/arp_tables.o
  CC      net/ipv4/netfilter/arpt_mangle.o
  CC      kernel/configs.o
  CC      net/ipv4/netfilter/arptable_filter.o
  CC      fs/f2fs/segment.o
  CC      drivers/i2c/i2c-dev.o
  LD      net/ipv4/netfilter/nf_conntrack_ipv4.o
  LD      net/ipv4/netfilter/nf_nat_ipv4.o
  LD      drivers/i2c/algos/built-in.o
  CC      net/netfilter/nf_conntrack_netbios_ns.o
  CC      drivers/i2c/busses/i2c-qup.o
  LD      drivers/idle/built-in.o
  LD      drivers/ieee802154/built-in.o
  CC      drivers/input/input.o
  CC      drivers/input/input-compat.o
  CC [M]  net/mac80211/rc80211_minstrel.o
  CC      drivers/input/input-mt.o
  CC      drivers/input/ff-core.o
  CC      net/netfilter/nf_conntrack_pptp.o
  CC      net/netfilter/nf_conntrack_sane.o
  CC      fs/f2fs/recovery.o
  CC      fs/fuse/file.o
  CC      fs/fuse/inode.o
  CC      fs/fuse/control.o
  CC      net/netfilter/nf_conntrack_tftp.o
  LD      net/netfilter/nf_nat.o
  CC      net/netfilter/nf_nat_proto_dccp.o
  CC [M]  net/mac80211/rc80211_minstrel_ht.o
  CC      drivers/input/ff-memless.o
  CC      net/netfilter/nf_nat_proto_udplite.o
  CC      net/netfilter/nf_nat_proto_sctp.o
  LD      drivers/i2c/muxes/built-in.o
  CC      net/netfilter/nf_nat_amanda.o
  CC      net/netfilter/nf_nat_ftp.o
  LD      kernel/built-in.o
  CC      drivers/input/mousedev.o
  CC      drivers/input/joydev.o
  CC      drivers/input/evdev.o
  CC      drivers/input/joystick/xpad.o
  CC      net/netfilter/nf_nat_irc.o
  CC      drivers/input/keyboard/atkbd.o
  CC      drivers/input/keyboard/gpio_keys.o
  LD      drivers/i2c/busses/built-in.o
  LD      drivers/i2c/built-in.o
  CC      drivers/input/keyboard/matrix_keypad.o
  CC      net/netfilter/nf_nat_tftp.o
  CC      fs/f2fs/shrinker.o
  CC      net/netfilter/nf_tproxy_core.o
  CC      net/netfilter/x_tables.o
  CC      net/netfilter/xt_tcpudp.o
  CC      drivers/input/misc/keychord.o
  CC      net/netfilter/xt_mark.o
  LD      net/ipv4/netfilter/built-in.o
  CC      drivers/input/misc/mpu3050.o
  LD      net/ipv4/built-in.o
  CC      drivers/input/mouse/psmouse-base.o
  CC      drivers/input/misc/uinput.o
  CC      drivers/input/misc/lis3dh_acc.o
  CC      net/netfilter/xt_connmark.o
  CC      net/netfilter/xt_nat.o
  CC      net/netfilter/xt_CLASSIFY.o
  LD      drivers/input/joystick/built-in.o
  CC      drivers/input/lid.o
  CC      drivers/input/touchscreen/ektf3k.o
  CC      net/netfilter/xt_CONNSECMARK.o
  CC      net/netlink/af_netlink.o
  CC      fs/f2fs/extent_cache.o
  CC      net/netlink/genetlink.o
  CC      net/netfilter/xt_CT.o
  CC      net/netfilter/xt_HMARK.o
  CC      net/netfilter/xt_LOG.o
  CC      net/netfilter/xt_NFLOG.o
  LD      drivers/input/keyboard/built-in.o
  LD      drivers/input/input-core.o
  CC      net/netfilter/xt_NFQUEUE.o
  CC      net/netfilter/xt_SECMARK.o
  CC      fs/jbd/transaction.o
  LD      fs/fuse/fuse.o
  LD      fs/fuse/built-in.o
  CC      fs/jbd/commit.o
  CC      fs/jbd2/transaction.o
  CC      fs/jbd2/commit.o
  CC      net/netfilter/xt_TCPMSS.o
  CC      net/netfilter/xt_IDLETIMER.o
  CC      net/netfilter/xt_comment.o
  CC      net/netfilter/xt_connlabel.o
  CC      net/netfilter/xt_connlimit.o
  CC      drivers/input/serio/serio.o
  CC      drivers/input/serio/serport.o
  CC      drivers/input/mouse/synaptics.o
  CC      net/netfilter/xt_conntrack.o
  CC      net/netfilter/xt_ecn.o
  CC      net/netfilter/xt_hashlimit.o
  LD      drivers/input/misc/built-in.o
  CC      net/netfilter/xt_helper.o
  CC      net/netfilter/xt_hl.o
  CC      net/netfilter/xt_iprange.o
  CC      fs/f2fs/debug.o
  CC      net/netfilter/xt_length.o
  CC      net/netfilter/xt_limit.o
  CC      net/netfilter/xt_mac.o
  CC      net/packet/af_packet.o
  CC      drivers/input/serio/libps2.o
  CC      net/netfilter/xt_multiport.o
  CC      fs/jbd/recovery.o
  CC      fs/jbd/checkpoint.o
  CC      fs/jbd/revoke.o
  CC      fs/jbd/journal.o
  CC      net/netfilter/xt_pkttype.o
  CC      fs/jbd2/recovery.o
  CC      net/netfilter/xt_policy.o
  CC      fs/jbd2/checkpoint.o
  CC      net/netfilter/xt_qtaguid_print.o
  CC      net/netfilter/xt_qtaguid.o
  CC      net/netfilter/xt_quota.o
  CC      fs/jbd2/revoke.o
  CC      fs/jbd2/journal.o
  CC      net/netfilter/xt_quota2.o
  CC      fs/lockd/clntlock.o
  CC      drivers/input/mouse/alps.o
  CC      fs/f2fs/xattr.o
  CC      fs/lockd/clntproc.o
  CC      net/netfilter/xt_socket.o
  CC      net/netfilter/xt_state.o
  LD [M]  net/mac80211/mac80211.o
  CC      net/netfilter/xt_statistic.o
  LD      drivers/input/serio/built-in.o
  CC      net/netfilter/xt_string.o
  CC      net/netfilter/xt_time.o
  LD      net/netlink/built-in.o
  CC      net/netfilter/xt_u32.o
  CC      net/rfkill/core.o
  CC      drivers/iommu/iommu.o
  LD      net/netfilter/netfilter.o
  LD      drivers/input/touchscreen/built-in.o
  LD      net/netfilter/nfnetlink_queue.o
  LD      net/netfilter/nf_conntrack.o
  CC      drivers/iommu/msm_iommu.o
  CC      drivers/iommu/msm_iommu_dev.o
  CC      fs/lockd/clntxdr.o
  CC      fs/lockd/host.o
  CC      fs/nfs_common/nfsacl.o
  CC      fs/nls/nls_base.o
  CC      fs/notify/fsnotify.o
  CC      fs/nfs/client.o
  CC      fs/nls/nls_cp437.o
  CC      drivers/leds/led-core.o
  CC      fs/nls/nls_ascii.o
  CC      drivers/leds/led-class.o
  CC      drivers/leds/led-triggers.o
  CC      fs/f2fs/acl.o
  LD      drivers/lguest/built-in.o
  LD      drivers/macintosh/built-in.o
  CC      drivers/leds/leds-pm8xxx.o
  CC      drivers/input/mouse/logips2pp.o
  CC      drivers/input/mouse/trackpoint.o
  CC      fs/ntfs/aops.o
  CC      fs/nls/nls_iso8859-1.o
  LD      fs/nfs_common/nfs_acl.o
  CC      fs/lockd/svc.o
  LD      fs/nfs_common/built-in.o
  CC      fs/ntfs/attrib.o
  CC      fs/lockd/svclock.o
  CC      drivers/media/media-device.o
  CC      fs/notify/notification.o
  CC      fs/proc/mmu.o
  CC      drivers/media/media-devnode.o
  CC      fs/lockd/svcshare.o
  LD      net/rfkill/rfkill.o
  LD      fs/nls/built-in.o
  LD      net/rfkill/built-in.o
  CC      drivers/leds/ledtrig-heartbeat.o
  CC      drivers/mfd/mfd-core.o
  CC      drivers/mfd/wcd9xxx-core.o
  CC      drivers/mfd/wcd9xxx-irq.o
  CC      drivers/mfd/wcd9xxx-slimslave.o
  CC      drivers/mfd/pm8921-core.o
  LD      drivers/input/mouse/psmouse.o
  LD      drivers/iommu/built-in.o
  LD      drivers/input/mouse/built-in.o
  LD      drivers/input/built-in.o
  CC      drivers/misc/pmem.o
  CC      fs/lockd/svcproc.o
  CC      fs/proc/task_mmu.o
  LD      fs/f2fs/f2fs.o
  CC      drivers/mmc/card/block.o
  LD      fs/jbd/jbd.o
  LD      fs/f2fs/built-in.o
  LD      fs/jbd/built-in.o
  CC      fs/quota/dquot.o
  CC      fs/ramfs/inode.o
  LD      net/packet/built-in.o
  CC      fs/ramfs/file-mmu.o
  CC      drivers/media/media-entity.o
  CC      drivers/media/common/tuners/tuner-xc2028.o
  LD      drivers/leds/built-in.o
  LD      drivers/media/dvb/b2c2/built-in.o
  LD      drivers/media/dvb/bt8xx/built-in.o
  LD      drivers/media/dvb/ddbridge/built-in.o
  CC      drivers/net/dummy.o
  LD      drivers/media/dvb/dm1105/built-in.o
  CC      fs/notify/group.o
  CC      drivers/media/dvb/dvb-core/dvbdev.o
  CC      drivers/net/mii.o
  CC      drivers/net/Space.o
  CC      fs/lockd/svcsubs.o
  CC      fs/lockd/mon.o
  CC      drivers/mfd/pm8821-core.o
  LD      net/netfilter/built-in.o
  LD      fs/ramfs/ramfs.o
  LD      fs/ramfs/built-in.o
  CC      drivers/mfd/pm8xxx-irq.o
  CC      fs/lockd/xdr.o
  CC      fs/notify/inode_mark.o
  CC      fs/sdcardfs/dentry.o
  CC      drivers/mfd/pm8038-core.o
  CC      fs/sdcardfs/file.o
  CC      fs/nfs/dir.o
  CC      net/sched/sch_generic.o
  CC      net/sched/sch_mq.o
  CC      fs/sdcardfs/inode.o
  LD      fs/jbd2/jbd2.o
  CC      fs/sdcardfs/main.o
  LD      fs/jbd2/built-in.o
  CC      fs/proc/inode.o
  CC      net/sched/sch_api.o
  CC      fs/ntfs/collate.o
  CC      drivers/mfd/pm8821-irq.o
  CC      drivers/net/loopback.o
  CC      drivers/media/dvb/dvb-core/dmxdev.o
  CC      drivers/mfd/pm8xxx-debug.o
  CC      fs/notify/mark.o
  CC      fs/sdcardfs/super.o
  CC      fs/lockd/grace.o
  CC      fs/ntfs/compress.o
  CC      fs/sdcardfs/lookup.o
  CC      drivers/mfd/pm8xxx-pwm.o
  LD      drivers/net/caif/built-in.o
  CC      drivers/mfd/pm8xxx-misc.o
  CC      net/sched/sch_blackhole.o
  CC      fs/proc/root.o
  CC      fs/lockd/clnt4xdr.o
  LD      drivers/net/ethernet/3com/built-in.o
  LD      drivers/net/ethernet/8390/built-in.o
  CC      fs/ntfs/debug.o
  LD      drivers/net/ethernet/adaptec/built-in.o
  CC      drivers/mfd/pm8xxx-spk.o
  LD      drivers/net/ethernet/alteon/built-in.o
  LD      drivers/net/ethernet/amd/built-in.o
  CC      fs/sdcardfs/mmap.o
  CC      drivers/misc/smsc_hub.o
  LD      drivers/net/ethernet/atheros/built-in.o
  LD      drivers/net/ethernet/broadcom/built-in.o
  CC      fs/sdcardfs/packagelist.o
  LD      drivers/net/ethernet/brocade/built-in.o
  LD      drivers/net/ethernet/chelsio/built-in.o
  LD      drivers/net/ethernet/cirrus/built-in.o
  CC      drivers/media/common/tuners/tuner-simple.o
  CC      drivers/media/common/tuners/tuner-types.o
  LD      drivers/net/ethernet/cisco/built-in.o
  CC      drivers/mmc/card/queue.o
  LD      drivers/net/ethernet/dec/built-in.o
  CC      fs/proc/base.o
  CC      fs/notify/vfsmount_mark.o
  LD      drivers/net/ethernet/dlink/built-in.o
  LD      drivers/net/ethernet/emulex/built-in.o
  LD      drivers/net/ethernet/faraday/built-in.o
  CC      fs/sdcardfs/derived_perm.o
  LD      drivers/net/ethernet/hp/built-in.o
  LD      drivers/net/ethernet/i825xx/built-in.o
  CC      fs/lockd/xdr4.o
  LD      drivers/net/ethernet/intel/built-in.o
  LD      drivers/net/ethernet/marvell/built-in.o
  CC      fs/ntfs/dir.o
  LD      drivers/net/ethernet/mellanox/built-in.o
  CC      fs/lockd/svc4proc.o
  LD      drivers/net/ethernet/micrel/built-in.o
  LD      drivers/net/ethernet/microchip/built-in.o
  CC      drivers/net/ethernet/msm/msm_rmnet_bam.o
  CC      fs/proc/generic.o
  LD      drivers/net/ethernet/myricom/built-in.o
  LD      drivers/net/ethernet/natsemi/built-in.o
  LD      drivers/net/ethernet/neterion/built-in.o
  LD      drivers/net/ethernet/nvidia/built-in.o
  CC      fs/nfs/file.o
  CC      fs/quota/quota.o
  LD      drivers/net/ethernet/oki-semi/built-in.o
  CC      net/sched/cls_api.o
  CC      drivers/misc/uid_stat.o
  LD      drivers/net/ethernet/packetengines/built-in.o
  LD      drivers/net/ethernet/qlogic/built-in.o
  LD      drivers/net/ethernet/rdc/built-in.o
  LD      drivers/net/ethernet/realtek/built-in.o
  LD      drivers/net/ethernet/seeq/built-in.o
  CC      fs/notify/dnotify/dnotify.o
  LD      drivers/net/ethernet/silan/built-in.o
  CC      drivers/mfd/pm8xxx-batt-alarm.o
  LD      drivers/net/ethernet/sis/built-in.o
  CC      drivers/net/ethernet/smsc/smc91x.o
  LD      fs/notify/fanotify/built-in.o
  CC      fs/sysfs/inode.o
  CC      drivers/media/dvb/dvb-core/dvb_demux.o
  CC      fs/notify/inotify/inotify_fsnotify.o
  CC      fs/notify/inotify/inotify_user.o
  CC      drivers/net/ethernet/smsc/smc911x.o
  CC      drivers/net/ethernet/smsc/smsc911x.o
  LD      drivers/misc/carma/built-in.o
  LD      drivers/misc/cb710/built-in.o
  LD      drivers/misc/lis3lv02d/built-in.o
  CC      drivers/misc/eeprom/eeprom_93cx6.o
  CC      drivers/misc/slimport_anx7808/slimport.o
  CC      drivers/misc/slimport_anx7808/slimport_tx_drv.o
  LD      drivers/mmc/card/mmc_block.o
  LD      fs/notify/dnotify/built-in.o
  LD      drivers/mmc/card/built-in.o
  LD      fs/quota/built-in.o
  LD      fs/lockd/lockd.o
  CC      fs/eventpoll.o
  LD      drivers/misc/tspdrv/built-in.o
  LD      drivers/misc/ti-st/built-in.o
  CC      net/sched/act_api.o
  CC      drivers/misc/pm8xxx-vibrator.o
  CC      drivers/misc/qseecom.o
  CC      drivers/mmc/core/core.o
  LD      fs/lockd/built-in.o
  CC      net/sunrpc/clnt.o
  CC      fs/ntfs/file.o
  CC      drivers/net/ethernet/msm/msm_rmnet_smux.o
  CC      fs/sysfs/file.o
  CC      drivers/media/common/tuners/mt20xx.o
  CC      net/sunrpc/xprt.o
  LD      drivers/mfd/built-in.o
  LD      drivers/misc/eeprom/built-in.o
  LD      fs/notify/inotify/built-in.o
  CC      drivers/misc/uid_cputime.o
  CC      drivers/nfc/bcm2079x-i2c.o
  LD      fs/notify/built-in.o
  CC      fs/nfs/getroot.o
  CC      fs/nfs/inode.o
  CC      drivers/media/dvb/dvb-core/dvb_filter.o
  CC      drivers/media/dvb/dvb-core/dvb_ca_en50221.o
  CC      net/sched/sch_fifo.o
  CC      fs/proc/array.o
  CC      drivers/media/dvb/dvb-core/dvb_frontend.o
  LD      fs/sdcardfs/sdcardfs.o
  CC      drivers/media/dvb/dvb-core/dvb_net.o
  LD      fs/sdcardfs/built-in.o
  CC      fs/anon_inodes.o
  LD      drivers/nfc/built-in.o
  CC      drivers/pci/access.o
  CC      fs/signalfd.o
  CC      fs/sysfs/dir.o
  LD      drivers/net/ethernet/msm/built-in.o
  LD      drivers/net/ethernet/stmicro/built-in.o
  CC      fs/sysfs/symlink.o
  CC      fs/sysfs/mount.o
  LD      drivers/net/ethernet/sun/built-in.o
  CC      fs/nfs/super.o
  CC      drivers/media/common/tuners/tda8290.o
  CC      drivers/media/dvb/dvb-core/dvb_ringbuffer.o
  CC      drivers/media/dvb/dvb-core/dvb_math.o
  CC      drivers/media/common/tuners/tea5767.o
  CC      net/sched/sch_htb.o
  CC      fs/proc/proc_tty.o
  CC      fs/timerfd.o
  CC      fs/eventfd.o
  CC      net/sched/sch_prio.o
  CC      fs/sysfs/bin.o
  LD      drivers/net/ethernet/tehuti/built-in.o
  LD      drivers/media/dvb/dvb-usb/built-in.o
  LD      drivers/net/ethernet/ti/built-in.o
  LD      drivers/net/ethernet/via/built-in.o
  CC      drivers/media/dvb/frontends/rtl2830.o
  LD      drivers/media/dvb/mantis/built-in.o
  LD      drivers/media/dvb/ngene/built-in.o
  CC      drivers/pci/bus.o
  LD      drivers/media/dvb/pluto2/built-in.o
  CC      net/sunrpc/socklib.o
  CC      drivers/media/platform/msm/camera_v2/msm.o
  LD      drivers/media/dvb/pt1/built-in.o
  LD      drivers/misc/slimport_anx7808/built-in.o
  LD      drivers/media/dvb/siano/built-in.o
  CC      net/sunrpc/xprtsock.o
  CC      fs/ntfs/index.o
  CC      drivers/media/platform/msm/camera_v2/camera/camera.o
  CC      drivers/media/platform/msm/camera_v2/isp/msm_isp.o
  CC      drivers/media/platform/msm/camera_v2/gemini/msm_gemini_dev.o
  CC      drivers/media/platform/msm/camera_v2/isp/msm_buf_mgr.o
  CC      fs/proc/cmdline.o
  CC      drivers/mmc/core/bus.o
  LD      drivers/misc/built-in.o
  CC      drivers/media/platform/msm/camera_v2/isp/msm_isp_util.o
  CC      drivers/media/platform/msm/camera_v2/isp/msm_isp_axi_util.o
  CC      drivers/media/common/tuners/tea5761.o
  CC      fs/aio.o
  CC      fs/nfs/nfs2xdr.o
  CC      fs/proc/consoles.o
  CC      drivers/media/common/tuners/tda9887.o
  CC      fs/sysfs/group.o
  CC      net/sched/cls_u32.o
  LD      drivers/media/dvb/dvb-core/dvb-core.o
  CC      fs/locks.o
  LD      drivers/media/dvb/dvb-core/built-in.o
  CC      fs/ntfs/inode.o
  LD      drivers/media/dvb/ttpci/built-in.o
  CC      drivers/media/platform/msm/camera_v2/isp/msm_isp_stats_util.o
  CC      drivers/net/phy/phy.o
  CC      drivers/pci/probe.o
  CC      drivers/media/platform/msm/camera_v2/gemini/msm_gemini_sync.o
  CC      drivers/mmc/core/host.o
  CC      fs/proc/cpuinfo.o
  CC [M]  drivers/media/dvb/frontends/dvb-pll.o
  LD      drivers/media/platform/msm/camera_v2/camera/built-in.o
  CC [M]  drivers/media/dvb/frontends/stv0299.o
  CC      net/sunrpc/sched.o
  CC      net/sched/cls_fw.o
  CC      fs/nfs/direct.o
  CC      drivers/media/platform/msm/camera_v2/ispif/msm_ispif.o
  CC      fs/proc/devices.o
  CC      fs/proc/interrupts.o
  LD      fs/sysfs/built-in.o
  CC      fs/proc/loadavg.o
  CC      drivers/media/platform/msm/camera_v2/msm_buf_mgr/msm_generic_buf_mgr.o
  CC      drivers/media/platform/msm/camera_v2/isp/msm_isp40.o
  CC      drivers/media/platform/msm/camera_v2/isp/msm_isp32.o
  CC      drivers/media/common/tuners/tda827x.o
  CC      fs/proc/meminfo.o
  CC      fs/nfs/pagelist.o
  CC      fs/proc/stat.o
  CC      fs/proc/uptime.o
  CC      net/sched/cls_flow.o
  CC      fs/proc/version.o
  CC [M]  drivers/media/dvb/frontends/au8522_dig.o
  CC      net/sunrpc/auth.o
  CC      drivers/mmc/core/mmc.o
  LD      drivers/media/platform/msm/camera_v2/msm_buf_mgr/built-in.o
  CC      drivers/media/platform/msm/camera_v2/msm_vb2/msm_vb2.o
  CC      net/sched/ematch.o
  CC      drivers/net/phy/phy_device.o
  CC      fs/proc/softirqs.o
  CC [M]  drivers/media/dvb/frontends/au8522_decoder.o
  CC      fs/proc/namespaces.o
  LD      drivers/net/ethernet/smsc/built-in.o
  CC      fs/proc/proc_sysctl.o
  LD      drivers/net/ethernet/built-in.o
  CC      fs/proc/proc_net.o
  CC      drivers/pci/remove.o
  CC      fs/proc/kmsg.o
  CC      drivers/net/ppp/ppp_generic.o
  CC      drivers/net/ppp/ppp_async.o
  CC      fs/binfmt_script.o
  LD      drivers/media/platform/msm/camera_v2/ispif/built-in.o
  LD      drivers/media/platform/msm/camera_v2/pproc/cpp/built-in.o
  LD      drivers/media/platform/msm/camera_v2/pproc/built-in.o
  CC      drivers/media/platform/msm/camera_v2/sensor/actuator/msm_actuator.o
  CC      drivers/media/platform/msm/camera_v2/sensor/cci/msm_cci.o
  CC      drivers/media/common/tuners/tda18271-maps.o
  LD      drivers/media/platform/msm/camera_v2/msm_vb2/built-in.o
  CC      fs/proc/page.o
  CC      drivers/media/common/tuners/tda18271-common.o
  CC      fs/ntfs/mft.o
  CC      drivers/media/platform/msm/camera_v2/gemini/msm_gemini_core.o
  CC [M]  drivers/media/dvb/frontends/cxd2820r_core.o
  CC      fs/ntfs/mst.o
  CC [M]  drivers/media/dvb/frontends/cxd2820r_c.o
  CC      fs/binfmt_elf.o
  CC      net/sched/em_cmp.o
  CC      net/sched/em_nbyte.o
  CC      fs/nfs/proc.o
  CC      drivers/pci/pci.o
  LD      drivers/media/platform/msm/camera_v2/isp/built-in.o
  CC      fs/nfs/read.o
  CC      net/sunrpc/auth_null.o
  CC      drivers/mmc/core/mmc_ops.o
  CC      net/sched/em_u32.o
  CC      net/sched/em_meta.o
  CC      drivers/media/common/tuners/tda18271-fe.o
  CC      drivers/media/common/tuners/xc5000.o
  CC      net/sunrpc/auth_unix.o
  CC      drivers/media/common/tuners/xc4000.o
  CC      drivers/media/platform/msm/camera_v2/gemini/msm_gemini_hw.o
  CC      drivers/net/phy/mdio_bus.o
  CC      drivers/media/common/tuners/mc44s803.o
  CC      drivers/net/ppp/bsd_comp.o
  CC      drivers/media/platform/msm/camera_v2/sensor/csid/msm_csid.o
  LD      drivers/media/platform/msm/camera_v2/sensor/cci/built-in.o
  CC      fs/mbcache.o
  CC      net/sched/em_text.o
  CC      fs/posix_acl.o
  LD      drivers/media/platform/msm/camera_v2/sensor/actuator/built-in.o
  CC      fs/xattr_acl.o
  CC      drivers/media/platform/msm/camera_v2/gemini/msm_gemini_platform.o
  CC [M]  drivers/media/dvb/frontends/cxd2820r_t.o
  CC      drivers/media/platform/msm/camera_v2/sensor/csiphy/msm_csiphy.o
  CC      net/sunrpc/auth_generic.o
  LD      fs/proc/proc.o
  LD      fs/proc/built-in.o
  CC      fs/dcookies.o
  CC      fs/nfs/symlink.o
  CC      net/sunrpc/svc.o
  CC      drivers/mmc/core/sd.o
  CC      drivers/net/ppp/ppp_deflate.o
  CC      drivers/net/ppp/ppp_mppe.o
  CC      drivers/net/ppp/ppp_synctty.o
  LD      net/sched/built-in.o
  LD      drivers/media/platform/msm/camera_v2/sensor/csid/built-in.o
  CC      drivers/net/ppp/pppox.o
  CC      drivers/net/ppp/pppoe.o
  LD      drivers/media/platform/msm/camera_v2/sensor/eeprom/built-in.o
  CC      drivers/media/platform/msm/camera_v2/sensor/flash/msm_led_flash.o
  CC      net/unix/af_unix.o
  LD      drivers/media/radio/built-in.o
  CC      drivers/media/platform/msm/camera_v2/sensor/flash/msm_led_trigger.o
  CC [M]  drivers/media/dvb/frontends/cxd2820r_t2.o
  LD      drivers/media/platform/msm/camera_v2/gemini/built-in.o
  CC [M]  drivers/media/dvb/frontends/drxd_firm.o
  CC [M]  drivers/media/dvb/frontends/drxd_hard.o
  CC [M]  drivers/media/dvb/frontends/drxk_hard.o
  LD      drivers/net/phy/libphy.o
  LD      drivers/media/platform/msm/camera_v2/sensor/csiphy/built-in.o
  LD      drivers/net/phy/built-in.o
  CC      drivers/media/platform/msm/camera_v2/sensor/io/msm_camera_io_util.o
  CC      net/unix/garbage.o
  CC      drivers/net/slip/slip.o
  CC [M]  drivers/media/dvb/frontends/stb0899_drv.o
  CC      drivers/net/ppp/pppolac.o
  CC      drivers/net/slip/slhc.o
  LD      drivers/media/common/tuners/tda18271.o
  CC      drivers/net/ppp/pppopns.o
  CC      fs/nfs/unlink.o
  CC      fs/ntfs/namei.o
  CC      fs/ntfs/runlist.o
  LD      drivers/media/platform/msm/camera_v2/sensor/flash/built-in.o
  CC      net/sunrpc/svcsock.o
  LD      drivers/media/common/tuners/built-in.o
  LD      drivers/pinctrl/built-in.o
  CC      drivers/media/platform/msm/camera_v2/sensor/msm_sensor.o
  LD      drivers/media/common/built-in.o
  CC      drivers/media/platform/msm/camera_v2/sensor/ov5693.o
  CC      net/sunrpc/svcauth.o
  CC      drivers/media/rc/keymaps/rc-adstech-dvb-t-pci.o
  CC      drivers/mmc/core/sd_ops.o
  CC      drivers/media/rc/keymaps/rc-alink-dtu-m.o
  CC      drivers/media/rc/keymaps/rc-anysee.o
  CC      drivers/media/rc/keymaps/rc-apac-viewcomp.o
  CC      fs/ntfs/super.o
  CC      drivers/media/rc/keymaps/rc-asus-pc39.o
  CC      drivers/media/platform/msm/camera_v2/sensor/io/msm_camera_cci_i2c.o
  CC      net/unix/sysctl_net_unix.o
  CC      drivers/pci/pci-driver.o
  CC      drivers/pci/search.o
  CC      drivers/media/rc/keymaps/rc-ati-tv-wonder-hd-600.o
  CC      drivers/media/platform/msm/camera_v2/sensor/mi1040.o
  CC      drivers/media/rc/keymaps/rc-ati-x10.o
  LD      drivers/net/ppp/built-in.o
  CC      drivers/media/rc/keymaps/rc-avermedia-a16d.o
  CC [M]  drivers/media/dvb/frontends/stb0899_algo.o
  CC      drivers/media/rc/keymaps/rc-avermedia.o
  CC      drivers/media/rc/keymaps/rc-avermedia-cardbus.o
  CC      net/sunrpc/svcauth_unix.o
  CC      net/sunrpc/addr.o
  CC      net/sunrpc/rpcb_clnt.o
  CC      drivers/media/rc/keymaps/rc-avermedia-dvbt.o
  CC      fs/nfs/write.o
  CC      drivers/media/rc/keymaps/rc-avermedia-m135a.o
  CC      drivers/mmc/core/sdio.o
  CC      drivers/media/rc/keymaps/rc-avermedia-m733a-rm-k6.o
  CC      drivers/media/rc/keymaps/rc-avermedia-rm-ks.o
  CC      drivers/media/rc/keymaps/rc-avertv-303.o
  CC      drivers/media/rc/keymaps/rc-azurewave-ad-tu700.o
  CC      drivers/media/rc/keymaps/rc-behold.o
  CC      drivers/media/platform/msm/camera_v2/sensor/io/msm_camera_qup_i2c.o
  CC [M]  drivers/media/dvb/frontends/stv0900_core.o
  CC      drivers/media/rc/keymaps/rc-behold-columbus.o
  CC      drivers/pci/pci-sysfs.o
  CC      drivers/media/rc/keymaps/rc-budget-ci-old.o
  CC [M]  drivers/media/dvb/frontends/stv0900_sw.o
  LD      drivers/net/slip/built-in.o
  CC      drivers/net/usb/rtl8150.o
  CC      drivers/media/rc/keymaps/rc-cinergy-1400.o
  CC      drivers/media/rc/keymaps/rc-cinergy.o
  CC      drivers/media/rc/keymaps/rc-dib0700-nec.o
  CC      drivers/media/rc/keymaps/rc-dib0700-rc5.o
  CC      drivers/mmc/core/sdio_ops.o
  CC      drivers/media/rc/keymaps/rc-digitalnow-tinytwin.o
  CC      drivers/media/rc/keymaps/rc-digittrade.o
  CC      drivers/media/rc/keymaps/rc-dm1105-nec.o
  CC      drivers/media/rc/keymaps/rc-dntv-live-dvb-t.o
  CC      drivers/pci/rom.o
  CC      drivers/media/rc/keymaps/rc-dntv-live-dvbt-pro.o
  CC      net/sunrpc/timer.o
  CC      drivers/media/rc/keymaps/rc-em-terratec.o
  CC      drivers/media/rc/keymaps/rc-encore-enltv2.o
  CC      drivers/media/rc/keymaps/rc-encore-enltv.o
  CC      drivers/media/platform/msm/camera_v2/sensor/io/msm_camera_i2c_mux.o
  LD      net/unix/unix.o
  CC [M]  drivers/media/dvb/frontends/stb6100.o
  LD      net/unix/built-in.o
  CC      drivers/media/rc/keymaps/rc-encore-enltv-fm53.o
  CC      net/sunrpc/xdr.o
  CC      drivers/media/rc/keymaps/rc-evga-indtube.o
  CC      drivers/media/rc/keymaps/rc-eztv.o
  CC      net/wireless/core.o
  CC      drivers/media/rc/keymaps/rc-flydvb.o
  CC      drivers/mmc/core/sdio_bus.o
  CC      drivers/media/rc/keymaps/rc-flyvideo.o
  CC      drivers/net/usb/asix.o
  CC      drivers/net/usb/cdc_ether.o
  CC      drivers/net/usb/net1080.o
  CC      drivers/net/usb/rndis_host.o
  CC      net/sunrpc/sunrpc_syms.o
  CC      drivers/net/usb/cdc_subset.o
  CC      drivers/pci/setup-res.o
  CC      drivers/net/usb/zaurus.o
  CC      net/wireless/sysfs.o
  CC      net/wireless/radiotap.o
  CC      net/sunrpc/cache.o
  CC      drivers/media/platform/msm/camera_v2/sensor/io/msm_camera_dt_util.o
  CC      drivers/media/rc/keymaps/rc-fusionhdtv-mce.o
  CC      drivers/media/rc/keymaps/rc-gadmei-rm008z.o
  CC      fs/ntfs/sysctl.o
  CC      drivers/media/rc/keymaps/rc-genius-tvgo-a11mce.o
  CC      fs/ntfs/unistr.o
  CC      drivers/media/rc/keymaps/rc-gotview7135.o
  CC      drivers/mmc/core/sdio_cis.o
  CC      drivers/mmc/core/sdio_io.o
  CC [M]  drivers/media/dvb/frontends/sp8870.o
  CC      drivers/media/rc/keymaps/rc-imon-mce.o
  CC [M]  drivers/media/dvb/frontends/cx22700.o
  CC      drivers/mmc/core/sdio_irq.o
  CC      drivers/media/rc/keymaps/rc-imon-pad.o
  CC [M]  drivers/media/dvb/frontends/s5h1432.o
  CC      fs/nfs/namespace.o
  CC      drivers/net/usb/usbnet.o
  CC      drivers/net/usb/cdc_ncm.o
  CC      drivers/pci/irq.o
  CC      drivers/media/rc/keymaps/rc-iodata-bctv7e.o
  CC      drivers/media/rc/keymaps/rc-it913x-v1.o
  LD      drivers/media/platform/msm/camera_v2/sensor/io/built-in.o
  LD      drivers/media/platform/msm/camera_v2/sensor/built-in.o
  CC      drivers/media/rc/keymaps/rc-it913x-v2.o
  LD      drivers/media/platform/msm/camera_v2/built-in.o
  CC      drivers/media/rc/keymaps/rc-kaiomy.o
  CC      drivers/media/rc/keymaps/rc-kworld-315u.o
  CC      net/sunrpc/rpc_pipe.o
  LD      drivers/media/platform/msm/built-in.o
  CC      drivers/net/usb/rmnet_usb_ctrl.o
  LD      drivers/media/platform/built-in.o
  CC      fs/ntfs/upcase.o
  CC      net/sunrpc/svc_xprt.o
  CC      drivers/media/rc/keymaps/rc-kworld-pc150u.o
  CC      drivers/media/video/v4l2-dev.o
  CC      net/wireless/util.o
  CC      drivers/media/video/v4l2-ioctl.o
  CC      drivers/media/video/v4l2-device.o
  CC      drivers/media/rc/keymaps/rc-kworld-plus-tv-analog.o
  CC      drivers/media/rc/keymaps/rc-leadtek-y04g0051.o
  CC      drivers/media/rc/keymaps/rc-lirc.o
  CC      drivers/media/rc/keymaps/rc-lme2510.o
  CC      drivers/mmc/core/quirks.o
  CC      drivers/net/usb/rmnet_usb_data.o
  CC      drivers/mmc/core/cd-gpio.o
  CC      net/wireless/reg.o
  CC      drivers/pci/vpd.o
  CC [M]  drivers/media/dvb/frontends/cx24110.o
  CC [M]  drivers/media/dvb/frontends/tda8083.o
  CC [M]  drivers/media/dvb/frontends/l64781.o
  CC      net/xfrm/xfrm_policy.o
  CC      fs/nfs/mount_clnt.o
  CC      fs/ntfs/bitmap.o
  CC      net/xfrm/xfrm_state.o
  CC      drivers/media/rc/keymaps/rc-manli.o
  CC      net/xfrm/xfrm_hash.o
  CC      net/xfrm/xfrm_input.o
  CC      drivers/mmc/core/debugfs.o
  CC      net/xfrm/xfrm_output.o
  CC      drivers/media/rc/keymaps/rc-medion-x10.o
  CC      drivers/pci/proc.o
  CC      drivers/media/video/v4l2-fh.o
  CC      fs/ntfs/lcnalloc.o
  CC      drivers/media/video/v4l2-event.o
  CC [M]  drivers/media/dvb/frontends/dib3000mb.o
  CC [M]  drivers/media/dvb/frontends/dib3000mc.o
  CC [M]  drivers/media/dvb/frontends/dibx000_common.o
  CC      drivers/media/video/v4l2-ctrls.o
  CC      drivers/media/rc/keymaps/rc-msi-digivox-ii.o
  CC      fs/nfs/dns_resolve.o
  LD      drivers/mmc/core/mmc_core.o
  CC [M]  drivers/media/dvb/frontends/dib7000m.o
  LD      drivers/mmc/core/built-in.o
  CC [M]  drivers/media/dvb/frontends/dib7000p.o
  CC      drivers/mmc/host/msm_sdcc.o
  CC [M]  drivers/media/dvb/frontends/dib8000.o
  LD      drivers/net/usb/rmnet_usb.o
  CC [M]  drivers/media/dvb/frontends/dib9000.o
  LD      drivers/net/usb/built-in.o
  CC      drivers/media/rc/keymaps/rc-msi-digivox-iii.o
  CC      drivers/net/tun.o
  CC      drivers/pci/slot.o
  CC      net/sunrpc/stats.o
  CC      drivers/net/wireless/ath/ath6kl/debug.o
  CC      drivers/net/wireless/ath/ath6kl/hif.o
  CC      drivers/net/wireless/ath/ath6kl/htc.o
  LD      drivers/net/wireless/ath/ath9k/built-in.o
  CC      fs/ntfs/logfile.o
  CC [M]  drivers/net/wireless/ath/ath9k/beacon.o
  CC      drivers/media/video/v4l2-subdev.o
  CC      drivers/media/rc/keymaps/rc-msi-tvanywhere.o
  CC [M]  drivers/media/dvb/frontends/mt312.o
  CC      fs/nfs/cache_lib.o
  CC      net/xfrm/xfrm_algo.o
  CC      net/wireless/scan.o
  CC      drivers/media/rc/keymaps/rc-msi-tvanywhere-plus.o
  CC [M]  drivers/media/dvb/frontends/ves1820.o
  CC      drivers/pci/quirks.o
  CC [M]  drivers/media/dvb/frontends/ves1x93.o
  CC      fs/nfs/nfs3proc.o
  CC      drivers/media/rc/keymaps/rc-nebula.o
  CC      fs/ntfs/quota.o
  CC      drivers/media/video/v4l2-int-device.o
  CC      fs/nfs/nfs3xdr.o
  CC      fs/nfs/nfs3acl.o
  CC [M]  drivers/net/wireless/ath/ath9k/gpio.o
  CC      drivers/net/wireless/ath/ath6kl/bmi.o
  CC [M]  drivers/media/dvb/frontends/tda1004x.o
  CC      net/sunrpc/sysctl.o
  CC      drivers/media/rc/keymaps/rc-nec-terratec-cinergy-xs.o
  CC [M]  drivers/media/dvb/frontends/sp887x.o
  CC      net/xfrm/xfrm_sysctl.o
  CC      fs/ntfs/usnjrnl.o
  CC      drivers/media/video/v4l2-common.o
  CC [M]  drivers/media/dvb/frontends/nxt6000.o
  CC      net/xfrm/xfrm_replay.o
  CC      drivers/media/rc/keymaps/rc-norwood.o
  CC      drivers/media/rc/keymaps/rc-npgtech.o
  CC      net/xfrm/xfrm_ipcomp.o
  CC      drivers/media/video/videobuf2-core.o
  CC      drivers/media/video/videobuf2-memops.o
  CC [M]  drivers/media/dvb/frontends/mt352.o
  LD      fs/ntfs/ntfs.o
  CC      drivers/media/rc/keymaps/rc-pctv-sedna.o
  LD      fs/ntfs/built-in.o
  CC [M]  drivers/net/wireless/ath/ath9k/init.o
  CC      drivers/media/rc/keymaps/rc-philips.o
  CC      drivers/media/rc/keymaps/rc-pinnacle-color.o
  CC      fs/nfs/nfs4proc.o
  CC      net/sunrpc/auth_gss/auth_gss.o
  CC      net/sunrpc/auth_gss/gss_generic_token.o
  CC      drivers/media/video/videobuf2-vmalloc.o
  CC [M]  drivers/media/dvb/frontends/zl10036.o
  CC      drivers/net/wireless/ath/ath6kl/cfg80211.o
  CC [M]  drivers/media/dvb/frontends/zl10039.o
  CC [M]  drivers/media/dvb/frontends/zl10353.o
  CC      drivers/media/rc/keymaps/rc-pinnacle-grey.o
  CC      drivers/media/rc/keymaps/rc-pinnacle-pctv-hd.o
  CC      drivers/media/rc/keymaps/rc-pixelview.o
  CC      net/wireless/nl80211.o
  CC [M]  drivers/media/dvb/frontends/cx22702.o
  CC      fs/nfs/nfs4xdr.o
  CC      drivers/pci/hotplug.o
  CC      drivers/media/video/videobuf2-dma-contig.o
  CC      drivers/media/video/videobuf2-dma-sg.o
  LD [M]  drivers/media/dvb/frontends/drxd.o
  CC [M]  drivers/media/dvb/frontends/tda10021.o
  CC [M]  drivers/media/dvb/frontends/tda10023.o
  CC      drivers/media/rc/keymaps/rc-pixelview-mk12.o
  CC      net/sunrpc/auth_gss/gss_mech_switch.o
  CC      drivers/media/rc/keymaps/rc-pixelview-002t.o
  CC      drivers/media/rc/keymaps/rc-pixelview-new.o
  CC [M]  drivers/media/dvb/frontends/stv0297.o
  CC      drivers/media/video/videobuf2-msm-mem.o
  CC [M]  drivers/media/dvb/frontends/nxt200x.o
  CC [M]  drivers/media/dvb/frontends/or51211.o
  CC      drivers/media/rc/keymaps/rc-powercolor-real-angel.o
  CC [M]  drivers/media/dvb/frontends/or51132.o
  CC      drivers/pci/msi.o
  CC      drivers/media/rc/keymaps/rc-proteus-2309.o
  LD      net/xfrm/built-in.o
  CC [M]  drivers/net/wireless/ath/ath9k/main.o
  CC      drivers/media/rc/keymaps/rc-purpletv.o
  CC      drivers/media/rc/keymaps/rc-pv951.o
  LD      drivers/media/video/davinci/built-in.o
  CC      drivers/media/video/gspca/gspca.o
  CC [M]  drivers/media/dvb/frontends/bcm3510.o
  CC      drivers/media/rc/keymaps/rc-hauppauge.o
  CC      drivers/media/rc/keymaps/rc-rc6-mce.o
  CC      drivers/media/rc/keymaps/rc-real-audio-220-32-keys.o
  CC      drivers/media/video/msm_wfd/wfd-ioctl.o
  CC [M]  drivers/media/dvb/frontends/s5h1420.o
  CC      drivers/media/video/msm_wfd/wfd-util.o
  CC      net/sunrpc/auth_gss/svcauth_gss.o
  CC      drivers/media/video/uvc/uvc_driver.o
  CC      drivers/media/video/msm_wfd/vsg-subdev.o
  CC [M]  drivers/media/dvb/frontends/lgdt330x.o
  CC      drivers/mmc/host/msm_sdcc_dml.o
  CC      drivers/media/rc/keymaps/rc-snapstream-firefly.o
  CC      drivers/media/rc/keymaps/rc-samsung-necx.o
  CC      drivers/media/video/vcap_v4l2.o
  CC [M]  drivers/media/dvb/frontends/lgdt3305.o
  CC [M]  drivers/media/dvb/frontends/cx24123.o
  CC [M]  drivers/media/dvb/frontends/lnbp21.o
  CC [M]  drivers/media/dvb/frontends/lnbp22.o
  CC      drivers/net/wireless/hostap/hostap_80211_rx.o
  CC      drivers/media/video/msm_wfd/mdp-dummy-subdev.o
  CC      drivers/net/wireless/hostap/hostap_80211_tx.o
  CC      drivers/media/rc/keymaps/rc-streamzap.o
  LD      drivers/mmc/host/built-in.o
  LD      drivers/mmc/built-in.o
  CC      drivers/net/wireless/hostap/hostap_ap.o
  CC      drivers/media/rc/keymaps/rc-tbs-nec.o
  CC      drivers/pci/setup-bus.o
  CC      drivers/media/video/msm_wfd/enc-mfc-subdev.o
  CC [M]  drivers/media/dvb/frontends/isl6405.o
  CC      drivers/media/rc/keymaps/rc-technisat-usb2.o
  CC [M]  drivers/media/dvb/frontends/isl6421.o
  CC      drivers/media/rc/keymaps/rc-terratec-cinergy-xs.o
  CC [M]  drivers/media/dvb/frontends/tda10086.o
  CC      drivers/net/wireless/ath/ath6kl/init.o
  CC [M]  drivers/media/dvb/frontends/tda826x.o
  CC      drivers/net/wireless/hostap/hostap_info.o
  CC [M]  drivers/net/wireless/ath/ath9k/recv.o
  CC      drivers/net/wireless/hostap/hostap_ioctl.o
  CC      drivers/net/wireless/hostap/hostap_main.o
  CC      drivers/media/rc/keymaps/rc-terratec-slim.o
  CC      drivers/net/wireless/hostap/hostap_proc.o
  LD      drivers/net/wireless/ath/carl9170/built-in.o
  CC [M]  drivers/net/wireless/ath/carl9170/main.o
  CC [M]  drivers/media/dvb/frontends/tda8261.o
  CC [M]  drivers/media/dvb/frontends/dib0070.o
  CC [M]  drivers/net/wireless/ath/carl9170/usb.o
  CC [M]  drivers/net/wireless/ath/carl9170/cmd.o
  LD      net/sunrpc/auth_gss/auth_rpcgss.o
  LD      net/sunrpc/auth_gss/built-in.o
  LD      net/sunrpc/sunrpc.o
  CC [M]  drivers/net/wireless/ath/carl9170/mac.o
  CC      drivers/media/rc/keymaps/rc-terratec-slim-2.o
  LD      drivers/media/video/gspca/gspca_main.o
  LD      drivers/media/video/gspca/built-in.o
  CC      drivers/media/video/uvc/uvc_queue.o
  CC      drivers/media/video/vcap_vc.o
  LD      net/sunrpc/built-in.o
  CC [M]  drivers/media/dvb/frontends/dib0090.o
  CC [M]  drivers/net/wireless/ath/carl9170/phy.o
  CC      fs/nfs/nfs4renewd.o
  CC      fs/nfs/nfs4state.o
  CC      drivers/media/rc/keymaps/rc-tevii-nec.o
  CC      drivers/pci/setup-irq.o
  CC      fs/nfs/delegation.o
  LD      drivers/media/video/msm_wfd/built-in.o
  CC [M]  drivers/media/dvb/frontends/tua6100.o
  CC      drivers/media/video/vcap_vp.o
  CC      drivers/media/video/ir-kbd-i2c.o
  CC [M]  drivers/net/wireless/ath/carl9170/led.o
  CC      drivers/media/video/uvc/uvc_v4l2.o
  CC      drivers/media/rc/keymaps/rc-tivo.o
  CC      drivers/media/rc/keymaps/rc-total-media-in-hand.o
  LD      drivers/media/video/videodev.o
  CC      drivers/media/rc/keymaps/rc-trekstor.o
  CC      drivers/pci/syscall.o
  CC      drivers/media/rc/keymaps/rc-tt-1500.o
  CC [M]  drivers/media/dvb/frontends/s5h1409.o
  CC      drivers/media/rc/keymaps/rc-twinhan1027.o
  CC      drivers/net/wireless/ath/ath6kl/main.o
  CC      fs/nfs/idmap.o
  CC      drivers/media/rc/keymaps/rc-ue-rf4ce.o
  CC      drivers/media/rc/keymaps/rc-videomate-m1f.o
  CC [M]  drivers/net/wireless/ath/carl9170/fw.o
  CC      drivers/media/rc/keymaps/rc-videomate-s350.o
  CC [M]  drivers/net/wireless/ath/ath9k/xmit.o
  CC [M]  drivers/net/wireless/ath/ath9k/mci.o
  CC      drivers/media/rc/keymaps/rc-videomate-tv-pvr.o
  CC [M]  drivers/media/dvb/frontends/itd1000.o
  CC [M]  drivers/net/wireless/ath/ath9k/pci.o
  CC      drivers/media/rc/keymaps/rc-winfast.o
  LD      drivers/pci/built-in.o
  CC [M]  drivers/net/wireless/ath/carl9170/tx.o
  CC [M]  drivers/net/wireless/ath/carl9170/rx.o
  CC      drivers/media/rc/keymaps/rc-winfast-usbii-deluxe.o
  CC      drivers/platform/msm/ssbi.o
  CC      drivers/platform/msm/sps/bam.o
  CC      drivers/power/power_supply_core.o
  CC      drivers/platform/msm/sps/sps_bam.o
  CC      drivers/power/power_supply_sysfs.o
  CC      drivers/net/wireless/ath/ath6kl/txrx.o
  CC      drivers/net/wireless/ath/ath6kl/wmi.o
  CC      drivers/media/video/uvc/uvc_video.o
  LD      drivers/media/rc/keymaps/built-in.o
  CC      drivers/media/rc/rc-main.o
  CC      drivers/media/rc/ir-raw.o
  LD      drivers/net/wireless/hostap/hostap.o
  CC      fs/nfs/callback.o
  LD      drivers/net/wireless/hostap/built-in.o
  CC      fs/nfs/callback_xdr.o
  LD [M]  drivers/media/dvb/frontends/au8522.o
  LD      drivers/net/wireless/rt2x00/built-in.o
  CC [M]  drivers/media/dvb/frontends/tda10048.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00dev.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00mac.o
  CC [M]  drivers/media/dvb/frontends/cx24113.o
  CC [M]  drivers/media/dvb/frontends/s5h1411.o
  CC [M]  drivers/media/dvb/frontends/lgs8gl5.o
  CC [M]  drivers/net/wireless/ath/ath9k/common.o
  CC      fs/nfs/callback_proc.o
  CC [M]  drivers/media/dvb/frontends/tda665x.o
  CC      drivers/power/power_supply_leds.o
  CC      fs/nfs/nfs4namespace.o
  CC      drivers/net/wireless/ath/ath6kl/core.o
  CC [M]  drivers/net/wireless/ath/ath6kl/usb.o
  CC      drivers/power/smb345-charger.o
  CC      net/wireless/mlme.o
  CC      drivers/media/rc/lirc_dev.o
  CC      fs/nfs/sysctl.o
  CC      drivers/media/rc/ir-nec-decoder.o
  LD [M]  drivers/net/wireless/ath/carl9170/carl9170.o
  CC [M]  drivers/media/dvb/frontends/lgs8gxx.o
  CC [M]  drivers/media/dvb/frontends/atbm8830.o
  CC      drivers/platform/msm/sps/sps.o
  CC      drivers/platform/msm/sps/sps_dma.o
  CC [M]  drivers/media/dvb/frontends/af9013.o
  CC      drivers/media/video/uvc/uvc_ctrl.o
  CC      drivers/media/video/uvc/uvc_status.o
  CC      drivers/net/wireless/ath/main.o
  CC [M]  drivers/media/dvb/frontends/cx24116.o
  CC [M]  drivers/media/dvb/frontends/si21xx.o
  CC [M]  drivers/media/dvb/frontends/stv0288.o
  CC [M]  drivers/media/dvb/frontends/stb6000.o
  CC [M]  drivers/net/wireless/ath/ath9k/htc_hst.o
  CC [M]  drivers/net/wireless/ath/ath9k/hif_usb.o
  LD [M]  drivers/net/wireless/ath/ath6kl/ath6kl_usb.o
  CC [M]  drivers/net/wireless/ath/ath9k/wmi.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00config.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00queue.o
  LD      fs/nfs/nfs.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00link.o
  CC      drivers/platform/msm/sps/sps_map.o
  LD      fs/nfs/built-in.o
  LD      fs/built-in.o
  CC      drivers/media/video/uvc/uvc_isight.o
  LD      drivers/net/wireless/ath/ath6kl/ath6kl_core.o
  CC [M]  drivers/media/dvb/frontends/s921.o
  LD      drivers/net/wireless/ath/ath6kl/built-in.o
  CC      drivers/platform/msm/sps/sps_mem.o
  CC      drivers/net/wireless/ath/regd.o
  CC      drivers/platform/msm/sps/sps_rm.o
  CC      drivers/media/rc/ir-rc5-decoder.o
  CC [M]  drivers/media/dvb/frontends/stv6110.o
  CC      drivers/net/wireless/ath/hw.o
  LD [M]  drivers/media/dvb/frontends/stv0900.o
  CC [M]  drivers/media/dvb/frontends/stv090x.o
  CC      drivers/power/bq27541_battery.o
  CC      net/wireless/ibss.o
  LD      drivers/power/power_supply.o
  CC      net/wireless/sme.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00crypto.o
  CC [M]  drivers/media/dvb/frontends/stv6110x.o
  CC [M]  drivers/net/wireless/ath/ath9k/htc_drv_txrx.o
  CC [M]  drivers/net/wireless/ath/ath9k/htc_drv_main.o
  CC [M]  drivers/media/dvb/frontends/isl6423.o
  CC      drivers/media/video/uvc/uvc_debugfs.o
  CC      drivers/media/video/uvc/uvc_entity.o
  CC [M]  drivers/media/dvb/frontends/ec100.o
  CC [M]  drivers/media/dvb/frontends/hd29l2.o
  CC [M]  drivers/media/dvb/frontends/ds3000.o
  CC [M]  drivers/media/dvb/frontends/mb86a16.o
  CC      drivers/media/rc/ir-rc6-decoder.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00firmware.o
  CC [M]  drivers/net/wireless/ath/ath9k/htc_drv_beacon.o
  CC [M]  drivers/net/wireless/ath/ath9k/htc_drv_init.o
  CC [M]  drivers/net/wireless/ath/ath9k/htc_drv_gpio.o
  CC [M]  drivers/media/dvb/frontends/mb86a20s.o
  LD      drivers/media/video/uvc/uvcvideo.o
  LD      drivers/media/video/uvc/built-in.o
  LD      drivers/media/video/built-in.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00leds.o
  LD      drivers/media/media.o
  CC [M]  drivers/media/dvb/frontends/ix2505v.o
  CC [M]  drivers/media/dvb/frontends/stv0367.o
  CC      drivers/net/wireless/ath/key.o
  LD [M]  drivers/media/dvb/frontends/cxd2820r.o
  LD [M]  drivers/media/dvb/frontends/drxk.o
  CC      drivers/media/rc/ir-jvc-decoder.o
  CC      drivers/media/rc/ir-sony-decoder.o
  CC [M]  drivers/media/dvb/frontends/tda18271c2dd.o
  CC [M]  drivers/net/wireless/rt2x00/rt2x00usb.o
  CC [M]  drivers/media/dvb/frontends/it913x-fe.o
  CC [M]  drivers/media/dvb/frontends/a8293.o
  LD      drivers/power/built-in.o
  CC [M]  drivers/media/dvb/frontends/tda10071.o
  CC      drivers/regulator/core.o
  CC      drivers/regulator/dummy.o
  CC [M]  drivers/media/dvb/frontends/m88rs2000.o
  CC      drivers/regulator/fixed-helper.o
  CC      drivers/regulator/msm-gpio-regulator.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9002_hw.o
  CC      drivers/media/rc/ir-rc5-sz-decoder.o
  LD      drivers/media/dvb/frontends/built-in.o
  LD [M]  drivers/media/dvb/frontends/stb0899.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9003_hw.o
  CC      drivers/media/rc/ir-sanyo-decoder.o
  CC [M]  drivers/net/wireless/ath/ath9k/hw.o
  LD      drivers/platform/msm/sps/built-in.o
  LD      drivers/platform/msm/built-in.o
  CC [M]  drivers/net/wireless/rt2x00/rt2800lib.o
  CC      net/wireless/chan.o
  CC [M]  drivers/net/wireless/rt2x00/rt2500usb.o
  CC [M]  drivers/net/wireless/rt2x00/rt73usb.o
  LD      drivers/platform/built-in.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9003_phy.o
  CC      drivers/rtc/rtc-lib.o
  CC      drivers/rtc/hctosys.o
  CC      drivers/rtc/class.o
  CC      drivers/regulator/pm8xxx-regulator.o
  CC      drivers/media/rc/ir-mce_kbd-decoder.o
  CC      drivers/media/rc/ir-lirc-codec.o
  CC      drivers/media/rc/user-rc-input.o
  CC      drivers/media/rc/gpio-ir-recv.o
  LD      drivers/net/wireless/ath/ath.o
  LD      drivers/media/rc/rc-core.o
  CC      drivers/rtc/interface.o
  CC      drivers/rtc/rtc-dev.o
  CC      drivers/rtc/rtc-proc.o
  CC      drivers/rtc/rtc-sysfs.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9002_phy.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar5008_phy.o
  CC [M]  drivers/net/wireless/rt2x00/rt2800usb.o
  LD [M]  drivers/net/wireless/rt2x00/rt2x00lib.o
  CC      drivers/rtc/rtc-pm8xxx.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9002_calib.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9003_calib.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9003_rtt.o
  CC      net/wireless/ethtool.o
  CC      net/wireless/mesh.o
  CC      net/wireless/wext-compat.o
  CC [M]  drivers/net/wireless/ath/ath9k/calib.o
  LD      drivers/media/rc/built-in.o
  CC      net/wireless/wext-sme.o
  CC [M]  drivers/net/wireless/ath/ath9k/eeprom.o
  CC [M]  drivers/net/wireless/ath/ath9k/eeprom_def.o
  CC [M]  drivers/net/wireless/ath/ath9k/eeprom_4k.o
  CC [M]  drivers/net/wireless/ath/ath9k/eeprom_9287.o
  CC [M]  drivers/net/wireless/ath/ath9k/ani.o
  CC [M]  drivers/net/wireless/ath/ath9k/mac.o
  CC      net/wireless/lib80211.o
  CC      net/wireless/lib80211_crypt_wep.o
  LD      drivers/rtc/rtc-core.o
  LD      drivers/rtc/built-in.o
  CC      net/wireless/lib80211_crypt_ccmp.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9002_mac.o
  CC      drivers/scsi/scsi.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9003_mac.o
  CC      drivers/scsi/hosts.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9003_eeprom.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9003_paprd.o
  CC [M]  drivers/net/wireless/ath/ath9k/btcoex.o
  CC [M]  drivers/net/wireless/ath/ath9k/ar9003_mci.o
  CC      net/wireless/lib80211_crypt_tkip.o
  CC      net/wireless/wext-core.o
  CC      net/wireless/wext-proc.o
  CC      net/wireless/wext-spy.o
  LD      drivers/regulator/built-in.o
  CC      drivers/slimbus/slimbus.o
  CC      drivers/slimbus/slim-msm-ctrl.o
  CC      drivers/spi/spi.o
  CC      drivers/spi/spi_qsd.o
  CC      net/wireless/wext-priv.o
  LD      drivers/net/wireless/rtl818x/built-in.o
  CC      net/wireless/regdb.o
  LD      drivers/net/wireless/rtl818x/rtl8187/built-in.o
  CC [M]  drivers/net/wireless/rtl818x/rtl8187/dev.o
  CC      drivers/scsi/scsi_ioctl.o
  CC [M]  drivers/net/wireless/rtl818x/rtl8187/rtl8225.o
  LD      drivers/media/dvb/ttusb-budget/built-in.o
  LD      drivers/media/dvb/ttusb-dec/built-in.o
  LD      drivers/media/dvb/built-in.o
  CC [M]  drivers/net/wireless/rtl818x/rtl8187/leds.o
  CC [M]  drivers/net/wireless/rtl818x/rtl8187/rfkill.o
  CC      drivers/scsi/constants.o
  LD      drivers/media/built-in.o
  CC      drivers/scsi/scsicam.o
  CC      drivers/staging/staging.o
  CC      drivers/staging/android/binder.o
  CC      drivers/staging/android/ashmem.o
  CC      drivers/staging/android/persistent_ram.o
  CC      drivers/staging/android/ram_console.o
  CC      drivers/staging/android/timed_output.o
  CC      drivers/staging/android/timed_gpio.o
  LD      net/wireless/cfg80211.o
  LD      drivers/staging/media/built-in.o
  LD      net/wireless/built-in.o
  CC      drivers/switch/switch_class.o
  CC      net/sysctl_net.o
  CC      net/activity_stats.o
  CC      drivers/staging/qcache/qcache-main.o
  CC      drivers/staging/qcache/tmem.o
  LD      drivers/staging/serial/built-in.o
  CC      drivers/staging/qcache/fmem.o
  CC      drivers/scsi/scsi_error.o
  CC      drivers/scsi/scsi_lib.o
  CC      drivers/staging/android/lowmemorykiller.o
  CC      drivers/scsi/scsi_lib_dma.o
  CC      drivers/scsi/scsi_scan.o
  CC      drivers/scsi/scsi_sysfs.o
  CC      drivers/scsi/scsi_devinfo.o
  CC      drivers/scsi/scsi_sysctl.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiData.o
  LD      drivers/switch/built-in.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiDebug.o
  CC      drivers/thermal/thermal_sys.o
  CC      drivers/thermal/msm8960_tsens.o
  CC      drivers/tty/tty_io.o
  CC      drivers/thermal/pm8xxx-tm.o
  CC      drivers/tty/n_tty.o
  CC      drivers/tty/tty_ioctl.o
  CC      drivers/tty/tty_ldisc.o
  CC      drivers/tty/tty_buffer.o
  CC      drivers/tty/tty_port.o
  LD      net/built-in.o
  CC      drivers/scsi/scsi_proc.o
  LD      drivers/spi/built-in.o
  CC      drivers/uio/uio.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiExt.o
  LD      drivers/staging/qcache/qcache.o
  LD [M]  drivers/net/wireless/ath/ath9k/ath9k.o
  LD      drivers/staging/qcache/built-in.o
  LD [M]  drivers/net/wireless/ath/ath9k/ath9k_hw.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiHCBB.o
  LD [M]  drivers/net/wireless/ath/ath9k/ath9k_common.o
  LD [M]  drivers/net/wireless/ath/ath9k/ath9k_htc.o
  LD      drivers/slimbus/built-in.o
  CC      drivers/uio/msm_sharedmem.o
  LD      drivers/net/wireless/ath/built-in.o
  LD [M]  drivers/net/wireless/rtl818x/rtl8187/rtl8187.o
  CC      drivers/usb/class/cdc-acm.o
  CC      drivers/thermal/msm_thermal.o
  CC      drivers/usb/core/usb.o
  LD      drivers/net/wireless/rtlwifi/built-in.o
  CC [M]  drivers/net/wireless/rtlwifi/base.o
  CC      drivers/usb/core/hub.o
  CC      drivers/scsi/scsi_trace.o
  CC      drivers/scsi/scsi_pm.o
  CC      drivers/scsi/scsi_tgt_lib.o
  CC      drivers/scsi/scsi_tgt_if.o
  CC      drivers/scsi/sd.o
  CC      drivers/tty/tty_mutex.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiInfo.o
  CC      drivers/tty/pty.o
  CC      drivers/tty/tty_audit.o
  LD      drivers/scsi/arm/built-in.o
  CC      drivers/tty/sysrq.o
  CC      drivers/tty/n_smux.o
  CC      drivers/tty/smux_debug.o
  CC      drivers/scsi/sg.o
  CC      drivers/tty/smux_test.o
  LD      drivers/thermal/built-in.o
  CC      drivers/tty/smux_loopback.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiLinkCntl.o
  CC      drivers/scsi/ch.o
  LD      drivers/uio/built-in.o
  CC      drivers/video/fb_notify.o
  CC      drivers/tty/smux_ctl.o
  LD      drivers/tty/ipwireless/built-in.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiLinkSupervision.o
  CC      drivers/tty/serial/serial_core.o
  CC      drivers/tty/serial/msm_serial_hs.o
  CC      drivers/tty/serial/msm_serial_hs_lite.o
  CC      drivers/tty/vt/vt_ioctl.o
  CC      drivers/tty/vt/vc_screen.o
  CC      drivers/tty/vt/selection.o
  CC [M]  drivers/scsi/scsi_wait_scan.o
  CC      drivers/net/wireless/wcnss/wcnss_wlan.o
  CC      drivers/usb/host/pci-quirks.o
  CC      drivers/usb/gadget/udc-core.o
  LD      drivers/usb/class/built-in.o
  CC      drivers/usb/host/ehci-hcd.o
  CC      drivers/usb/misc/ehset.o
  CC      drivers/usb/misc/diag_bridge.o
  CC      drivers/usb/misc/mdm_ctrl_bridge.o
  CC      drivers/video/fbmem.o
  CC      drivers/usb/misc/mdm_data_bridge.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiStatus.o
  CC      drivers/tty/vt/keyboard.o
  CC [M]  drivers/net/wireless/rtlwifi/cam.o
  CC      drivers/tty/vt/consolemap.o
  CONMK   drivers/tty/vt/consolemap_deftbl.c
  CC      drivers/tty/vt/vt.o
  CC      drivers/usb/misc/ks_bridge.o
  SHIPPED drivers/tty/vt/defkeymap.c
  CC      drivers/tty/vt/consolemap_deftbl.o
  CC      drivers/usb/gadget/ci13xxx_msm.o
  CC      drivers/tty/vt/defkeymap.o
  CC      drivers/usb/gadget/android.o
  CC      drivers/usb/gadget/f_hid.o
  CC [M]  drivers/net/wireless/rtlwifi/core.o
  CC [M]  drivers/net/wireless/rtlwifi/debug.o
  CC      drivers/net/wireless/wcnss/wcnss_riva.o
  CC      drivers/net/wireless/wcnss/qcomwlan_secif.o
  CC      drivers/staging/prima/CORE/BAP/src/bapApiTimer.o
  CC      drivers/staging/prima/CORE/BAP/src/bapModule.o
  LD      drivers/scsi/scsi_mod.o
  CC      drivers/staging/prima/CORE/BAP/src/bapRsn8021xAuthFsm.o
  LD      drivers/scsi/scsi_tgt.o
  LD      drivers/scsi/sd_mod.o
  LD      drivers/scsi/built-in.o
  CC      drivers/staging/prima/CORE/BAP/src/bapRsn8021xPrf.o
  CC      drivers/staging/prima/CORE/BAP/src/bapRsn8021xSuppRsnFsm.o
  LD      drivers/tty/serial/built-in.o
  CC      drivers/staging/prima/CORE/BAP/src/bapRsnAsfPacket.o
  CC      drivers/staging/prima/CORE/BAP/src/bapRsnSsmAesKeyWrap.o
  CC      drivers/video/fbmon.o
  CC      drivers/video/fbcmap.o
  CC      drivers/video/fbsysfs.o
  CC      drivers/video/modedb.o
  CC      drivers/video/fbcvt.o
  CC      drivers/usb/core/hcd.o
  CC [M]  drivers/net/wireless/rtlwifi/efuse.o
  CC [M]  drivers/net/wireless/rtlwifi/ps.o
  LD      drivers/usb/misc/mdm_bridge.o
  LD      drivers/usb/misc/built-in.o
  CC [M]  drivers/net/wireless/rtlwifi/rc.o
  LD      drivers/staging/android/built-in.o
  CC      drivers/usb/otg/otg.o
  CC      drivers/usb/serial/usb-serial.o
  CC      drivers/usb/otg/msm_otg.o
  CC      drivers/usb/serial/generic.o
  LD      drivers/net/wireless/wcnss/wcnsscore.o
  LD      drivers/net/wireless/wcnss/built-in.o
  CC      drivers/net/wireless/rndis_wlan.o
  CC      drivers/staging/prima/CORE/BAP/src/bapRsnSsmEapol.o
  CC      drivers/staging/prima/CORE/BAP/src/bapRsnSsmReplayCtr.o
  CC [M]  drivers/net/wireless/at76c50x-usb.o
  CC      drivers/usb/serial/bus.o
  CC      drivers/video/backlight/lcd.o
  CC      drivers/video/backlight/backlight.o
  CC      drivers/staging/prima/CORE/BAP/src/bapRsnTxRx.o
  CC      drivers/video/console/dummycon.o
  CC      drivers/video/msm/msm_fb.o
  CC      drivers/video/msm/mdp.o
  CC      drivers/video/cfbfillrect.o
  LD      drivers/video/omap2/displays/built-in.o
  LD      drivers/video/omap2/built-in.o
  CC [M]  drivers/net/wireless/rtlwifi/regd.o
  CC      drivers/video/cfbcopyarea.o
  CC      drivers/staging/prima/CORE/BAP/src/btampFsm.o
  CC      drivers/usb/serial/sierra.o
  CC [M]  drivers/net/wireless/rtlwifi/pci.o
  CC      drivers/staging/prima/CORE/BAP/src/btampHCI.o
  LD      drivers/video/console/built-in.o
  CC      drivers/video/cfbimgblt.o
  CC      drivers/staging/prima/CORE/DXE/src/wlan_qct_dxe.o
  CC      drivers/usb/serial/csvt.o
  CC      drivers/video/backlight/generic_bl.o
  CC [M]  drivers/net/wireless/rtlwifi/usb.o
  LD      drivers/net/wireless/rtlwifi/rtl8192c/built-in.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192c/main.o
  LD      drivers/net/wireless/rtlwifi/rtl8192cu/built-in.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/dm.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/hw.o
  CC      drivers/video/sysfillrect.o
  CC      drivers/video/syscopyarea.o
  LD      drivers/usb/serial/usbserial.o
  CC      drivers/video/sysimgblt.o
  CC      drivers/usb/core/urb.o
  CC      drivers/video/fb_sys_fops.o
  CC      drivers/video/vfb.o
  CC      drivers/usb/core/message.o
  LD      drivers/tty/vt/built-in.o
  LD      drivers/usb/serial/built-in.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192c/dm_common.o
  LD      drivers/video/backlight/built-in.o
  CC      drivers/usb/storage/alauda.o
  LD      drivers/tty/built-in.o
  CC      drivers/usb/storage/cypress_atacb.o
  CC      drivers/usb/storage/datafab.o
  CC      drivers/usb/storage/freecom.o
  CC [M]  drivers/net/wireless/zd1201.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/led.o
  LD      drivers/video/fb.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/mac.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/phy.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/rf.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/sw.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/table.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192cu/trx.o
  CC      drivers/usb/core/driver.o
  CC      drivers/video/msm/mdp4_util.o
  CC      drivers/usb/storage/isd200.o
  CC      drivers/usb/storage/jumpshot.o
  CC      drivers/usb/storage/karma.o
  CC      drivers/staging/prima/CORE/DXE/src/wlan_qct_dxe_cfg_i.o
  CC      drivers/usb/storage/onetouch.o
  CC      drivers/staging/prima/CORE/HDD/src/bap_hdd_main.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_assoc.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_cfg.o
  CC      drivers/usb/storage/sddr09.o
  CC      drivers/video/msm/mdp4_overlay.o
  LD      drivers/usb/otg/built-in.o
  CC      drivers/usb/usb-common.o
  CC      drivers/video/msm/mdp4_overlay_lcdc.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_dev_pwr.o
  CC      drivers/usb/storage/sddr55.o
  CC      drivers/usb/storage/shuttle_usbat.o
  LD [M]  drivers/net/wireless/rtlwifi/rtlwifi.o
  CC      drivers/usb/storage/scsiglue.o
  CC      drivers/usb/storage/protocol.o
  CC      drivers/usb/storage/transport.o
  CC      drivers/usb/core/config.o
  CC      drivers/usb/storage/usb.o
  CC      drivers/usb/storage/initializers.o
  CC      drivers/usb/storage/sierra_ms.o
  CC      drivers/usb/storage/option_ms.o
  LD      drivers/usb/host/built-in.o
  CC      drivers/usb/storage/usual-tables.o
  CC      drivers/usb/core/file.o
  CC      drivers/usb/core/buffer.o
  CC      drivers/usb/core/sysfs.o
  LD [M]  drivers/net/wireless/rtlwifi/rtl8192cu/rtl8192cu.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192c/fw_common.o
  CC [M]  drivers/net/wireless/rtlwifi/rtl8192c/phy_common.o
  CC      drivers/usb/core/endpoint.o
  CC      drivers/video/msm/mdp4_overlay_dsi_video.o
  CC      drivers/video/msm/mdp4_overlay_dsi_cmd.o
  CC      drivers/video/msm/mdp4_dtv.o
  CC      drivers/video/msm/mdp4_overlay_dtv.o
  CC      drivers/video/msm/mdp_dma.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_dp_utils.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_early_suspend.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_ftm.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_hostapd.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_oemdata.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_main.o
  CC      drivers/usb/core/devio.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_mib.o
  CC      drivers/usb/core/notify.o
  CC      drivers/usb/core/generic.o
  CC      drivers/usb/core/quirks.o
  CC      drivers/usb/core/devices.o
  CC      drivers/usb/core/hcd-pci.o
  LD      drivers/usb/storage/usb-storage.o
  LD      drivers/usb/storage/ums-alauda.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_scan.o
  LD      drivers/usb/storage/ums-cypress.o
  LD      drivers/usb/storage/ums-datafab.o
  LD      drivers/usb/storage/ums-freecom.o
  LD      drivers/usb/storage/ums-isd200.o
  LD      drivers/usb/storage/ums-jumpshot.o
  LD      drivers/usb/storage/ums-karma.o
  LD      drivers/usb/storage/ums-onetouch.o
  LD      drivers/usb/storage/ums-sddr09.o
  CC      drivers/usb/core/inode.o
  LD      drivers/usb/storage/ums-sddr55.o
  LD      drivers/usb/storage/ums-usbat.o
  CC      drivers/video/msm/mdp_dma_s.o
  LD      drivers/usb/storage/built-in.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_softap_tx_rx.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_tx_rx.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_wext.o
  CC      drivers/video/msm/mdp_vsync.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_wmm.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_wowl.o
  CC      drivers/video/msm/mdp_cursor.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_cfg80211.o
  CC      drivers/video/msm/mdp_dma_tv.o
  CC      drivers/video/msm/msm_dss_io_8960.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_p2p.o
  CC      drivers/staging/prima/CORE/HDD/src/wlan_hdd_tdls.o
  CC      drivers/video/msm/mipi_dsi.o
  CC      drivers/video/msm/mipi_dsi_host.o
  CC      drivers/video/msm/mipi_novatek.o
  CC      drivers/video/msm/mipi_lg.o
  CC      drivers/video/msm/mipi_JDI.o
  CC      drivers/video/msm/msm_fb_panel.o
  CC      drivers/video/msm/mipi_novatek_1080P_pt.o
  CC      drivers/staging/prima/CORE/MAC/src/cfg/cfgApi.o
  CC      drivers/video/msm/mipi_lg_1080P_pt.o
  LD      drivers/usb/core/usbcore.o
  LD      drivers/usb/core/built-in.o
  CC      drivers/staging/prima/CORE/MAC/src/cfg/cfgDebug.o
  LD [M]  drivers/net/wireless/rtlwifi/rtl8192c/rtl8192c-common.o
  CC      drivers/staging/prima/CORE/MAC/src/cfg/cfgParamName.o
  CC      drivers/staging/prima/CORE/MAC/src/cfg/cfgProcMsg.o
  LD      drivers/net/wireless/built-in.o
  CC      drivers/staging/prima/CORE/MAC/src/cfg/cfgSendMsg.o
  CC      drivers/video/msm/mipi_JDI_1080P_pt.o
  CC      drivers/video/msm/hdmi_msm.o
  CC      drivers/video/msm/external_common.o
  LD      drivers/net/built-in.o
  CC      drivers/staging/prima/CORE/MAC/src/dph/dphHashTable.o
  CC      drivers/video/msm/vidc/common/init/vidc_init.o
  CC      drivers/video/msm/vidc/common/vcd/vcd_api.o
  CC      drivers/video/msm/vidc/common/vcd/vcd_power_sm.o
  CC      drivers/video/msm/vidc/common/vcd/vcd_client_sm.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limAIDmgmt.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limAdmitControl.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limApi.o
  CC      drivers/video/msm/vidc/common/vcd/vcd_device_sm.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limAssocUtils.o
  CC      drivers/video/msm/vidc/common/vcd/vcd_scheduler.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limDebug.o
  CC      drivers/video/msm/vidc/common/vcd/vcd_sub.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limFT.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limIbssPeerMgmt.o
  LD      drivers/video/msm/msm_mipi.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limLinkMonitoringAlgo.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limLogDump.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl_helper.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limP2P.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessActionFrame.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessAssocReqFrame.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl_utils.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl_interrupt_handler.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessAssocRspFrame.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessAuthFrame.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl_properties.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl_errors.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl_shared_mem.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessBeaconFrame.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessCfgUpdates.o
  CC      drivers/video/msm/vidc/1080p/ddl/vidc.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessDeauthFrame.o
  CC      drivers/video/msm/vidc/1080p/ddl/vidc_pix_cache.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessDisassocFrame.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessLmmMessages.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessMessageQueue.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessMlmReqMessages.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessMlmRspMessages.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessProbeReqFrame.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl_vidc.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessProbeRspFrame.o
  CC      drivers/video/msm/vidc/1080p/ddl/vcd_ddl_metadata.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessSmeReqMessages.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limPropExtsUtils.o
  CC      drivers/video/msm/vidc/1080p/resource_tracker/vcd_res_tracker.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limRoamingAlgo.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limScanResultUtils.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limSecurityUtils.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limSendManagementFrames.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limSendMessages.o
  CC      drivers/video/msm/vidc/common/dec/vdec.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limSendSmeRspMessages.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limSerDesUtils.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limSession.o
  CC      drivers/video/msm/vidc/common/enc/venc.o
  CC      drivers/video/msm/vidc/common/enc/venc_internal.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limSessionUtils.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limSmeReqUtils.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limStaHashApi.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limTimerUtils.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limTrace.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limUtils.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/lim/limProcessTdls.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/pmm/pmmAP.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/pmm/pmmApi.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/pmm/pmmDebug.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/sch/schApi.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/sch/schBeaconGen.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/sch/schBeaconProcess.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/sch/schDebug.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/sch/schMessage.o
  CC      drivers/staging/prima/CORE/MAC/src/pe/rrm/rrmApi.o
  CC      drivers/staging/prima/CORE/SAP/src/sapApiLinkCntl.o
  CC      drivers/staging/prima/CORE/SAP/src/sapChSelect.o
  CC      drivers/staging/prima/CORE/SAP/src/sapFsm.o
  CC      drivers/staging/prima/CORE/SAP/src/sapModule.o
  CC      drivers/staging/prima/CORE/SME/src/btc/btcApi.o
  CC      drivers/staging/prima/CORE/SME/src/ccm/ccmApi.o
  CC      drivers/staging/prima/CORE/SME/src/ccm/ccmLogDump.o
  CC      drivers/staging/prima/CORE/SME/src/sme_common/sme_Api.o
  CC      drivers/staging/prima/CORE/SME/src/sme_common/sme_FTApi.o
  CC      drivers/staging/prima/CORE/SME/src/csr/csrApiRoam.o
  CC      drivers/staging/prima/CORE/SME/src/csr/csrApiScan.o
  CC      drivers/staging/prima/CORE/SME/src/csr/csrCmdProcess.o
  CC      drivers/staging/prima/CORE/SME/src/csr/csrLinkList.o
  CC      drivers/staging/prima/CORE/SME/src/csr/csrLogDump.o
  CC      drivers/staging/prima/CORE/SME/src/csr/csrUtil.o
  CC      drivers/staging/prima/CORE/SME/src/csr/csrNeighborRoam.o
  CC      drivers/staging/prima/CORE/SME/src/csr/csrTdlsProcess.o
  CC      drivers/staging/prima/CORE/SME/src/oemData/oemDataApi.o
  CC      drivers/staging/prima/CORE/SME/src/p2p/p2p_Api.o
  CC      drivers/staging/prima/CORE/SME/src/pmc/pmcApi.o
  LD      drivers/video/msm/vidc/vidc.o
  LD      drivers/video/msm/vidc/vidc_vdec.o
  LD      drivers/video/msm/vidc/vidc_venc.o
  LD      drivers/video/msm/vidc/built-in.o
  LD      drivers/video/msm/built-in.o
  CC      drivers/staging/prima/CORE/SME/src/pmc/pmc.o
  CC      drivers/staging/prima/CORE/SME/src/pmc/pmcLogDump.o
  CC      drivers/staging/prima/CORE/SME/src/QoS/sme_Qos.o
  LD      drivers/video/built-in.o
  CC      drivers/staging/prima/CORE/SME/src/rrm/sme_rrm.o
  CC      drivers/staging/prima/CORE/SVC/src/btc/wlan_btc_svc.o
  CC      drivers/staging/prima/CORE/SVC/src/nlink/wlan_nlink_srv.o
  CC      drivers/staging/prima/CORE/SVC/src/ptt/wlan_ptt_sock_svc.o
  CC      drivers/staging/prima/CORE/SYS/common/src/wlan_qct_sys.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/pal/src/palApiComm.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/pal/src/palTimer.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/platform/src/VossWrapper.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/system/src/macInitApi.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/system/src/sysEntryFunc.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/utils/src/dot11f.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/utils/src/logApi.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/utils/src/logDump.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/utils/src/macTrace.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/utils/src/parserApi.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/utils/src/utilsApi.o
  CC      drivers/staging/prima/CORE/SYS/legacy/src/utils/src/utilsParser.o
  CC      drivers/staging/prima/CORE/TL/src/wlan_qct_tl.o
  CC      drivers/staging/prima/CORE/TL/src/wlan_qct_tl_ba.o
  CC      drivers/staging/prima/CORE/TL/src/wlan_qct_tl_hosupport.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_api.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_event.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_getBin.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_list.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_lock.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_memory.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_mq.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_nvitem.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_packet.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_power.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_sched.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_threads.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_timer.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_trace.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_types.o
  CC      drivers/staging/prima/CORE/VOSS/src/vos_utils.o
  CC      drivers/staging/prima/CORE/WDA/src/wlan_qct_wda.o
  CC      drivers/staging/prima/CORE/WDA/src/wlan_qct_wda_debug.o
  CC      drivers/staging/prima/CORE/WDA/src/wlan_qct_wda_ds.o
  CC      drivers/staging/prima/CORE/WDA/src/wlan_qct_wda_legacy.o
  CC      drivers/staging/prima/CORE/WDA/src/wlan_nv.o
  CC      drivers/staging/prima/CORE/WDI/CP/src/wlan_qct_wdi.o
  CC      drivers/staging/prima/CORE/WDI/CP/src/wlan_qct_wdi_dp.o
  CC      drivers/staging/prima/CORE/WDI/CP/src/wlan_qct_wdi_sta.o
  CC      drivers/staging/prima/CORE/WDI/DP/src/wlan_qct_wdi_bd.o
  CC      drivers/staging/prima/CORE/WDI/DP/src/wlan_qct_wdi_ds.o
  CC      drivers/staging/prima/CORE/WDI/TRP/CTS/src/wlan_qct_wdi_cts.o
  CC      drivers/staging/prima/CORE/WDI/TRP/DTS/src/wlan_qct_wdi_dts.o
  CC      drivers/staging/prima/CORE/WDI/WPAL/src/wlan_qct_pal_api.o
  CC      drivers/staging/prima/CORE/WDI/WPAL/src/wlan_qct_pal_device.o
  CC      drivers/staging/prima/CORE/WDI/WPAL/src/wlan_qct_pal_msg.o
  CC      drivers/staging/prima/CORE/WDI/WPAL/src/wlan_qct_pal_packet.o
  CC      drivers/staging/prima/CORE/WDI/WPAL/src/wlan_qct_pal_sync.o
  CC      drivers/staging/prima/CORE/WDI/WPAL/src/wlan_qct_pal_timer.o
  CC      drivers/staging/prima/CORE/WDI/WPAL/src/wlan_qct_pal_trace.o
  LD      drivers/usb/gadget/g_android.o
  LD      drivers/usb/gadget/built-in.o
  LD      drivers/usb/built-in.o
  LD      drivers/staging/prima/wlan.o
  LD      drivers/staging/prima/built-in.o
  LD      drivers/staging/built-in.o
  LD      drivers/built-in.o
  LD      vmlinux.o
  MODPOST vmlinux.o
  GEN     .version
  CHK     include/generated/compile.h
  UPD     include/generated/compile.h
  CC      init/version.o
  LD      init/built-in.o
  LD      .tmp_vmlinux1
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 25 of arch/arm/common/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 8 of arch/arm/crypto/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 138 of arch/arm/mach-msm/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 570 of mm/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 1123 of fs/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 51 of crypto/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 402 of block/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 303 of lib/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 74 of drivers/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 6 of sound/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 861 of net/built-in.o is not in EXIDX output section
  KSYM    .tmp_kallsyms1.S
  AS      .tmp_kallsyms1.o
  LD      .tmp_vmlinux2
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 25 of arch/arm/common/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 8 of arch/arm/crypto/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 138 of arch/arm/mach-msm/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 570 of mm/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 1123 of fs/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 51 of crypto/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 402 of block/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 303 of lib/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 74 of drivers/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 6 of sound/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 861 of net/built-in.o is not in EXIDX output section
  KSYM    .tmp_kallsyms2.S
  AS      .tmp_kallsyms2.o
  LD      vmlinux
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 25 of arch/arm/common/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 8 of arch/arm/crypto/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 138 of arch/arm/mach-msm/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 570 of mm/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 1123 of fs/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 51 of crypto/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 402 of block/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 303 of lib/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 74 of drivers/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 6 of sound/built-in.o is not in EXIDX output section
/root/pie9/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-ld: warning: unwinding may not work because EXIDX input section 861 of net/built-in.o is not in EXIDX output section
  SYSMAP  System.map
  SYSMAP  .tmp_System.map
  OBJCOPY arch/arm/boot/Image
  Building modules, stage 2.
  MODPOST 109 modules
  Kernel: arch/arm/boot/Image is ready
  AS      arch/arm/boot/compressed/head.o
  XZKERN  arch/arm/boot/compressed/piggy.xzkern
  CC      arch/arm/boot/compressed/misc.o
  CC      arch/arm/boot/compressed/decompress.o
  CC      arch/arm/boot/compressed/string.o
  SHIPPED arch/arm/boot/compressed/lib1funcs.S
  SHIPPED arch/arm/boot/compressed/ashldi3.S
  AS      arch/arm/boot/compressed/lib1funcs.o
  AS      arch/arm/boot/compressed/ashldi3.o
  CC      drivers/bluetooth/bcm203x.mod.o
  CC      drivers/bluetooth/bfusb.mod.o
  CC      drivers/bluetooth/bpa10x.mod.o
  CC      drivers/media/dvb/frontends/a8293.mod.o
  CC      drivers/media/dvb/frontends/af9013.mod.o
  CC      drivers/media/dvb/frontends/atbm8830.mod.o
  CC      drivers/media/dvb/frontends/au8522.mod.o
  CC      drivers/media/dvb/frontends/bcm3510.mod.o
  CC      drivers/media/dvb/frontends/cx22700.mod.o
  CC      drivers/media/dvb/frontends/cx22702.mod.o
  CC      drivers/media/dvb/frontends/cx24110.mod.o
  CC      drivers/media/dvb/frontends/cx24113.mod.o
  CC      drivers/media/dvb/frontends/cx24116.mod.o
  CC      drivers/media/dvb/frontends/cx24123.mod.o
  CC      drivers/media/dvb/frontends/cxd2820r.mod.o
  CC      drivers/media/dvb/frontends/dib0070.mod.o
  CC      drivers/media/dvb/frontends/dib0090.mod.o
  CC      drivers/media/dvb/frontends/dib3000mb.mod.o
  CC      drivers/media/dvb/frontends/dib3000mc.mod.o
  CC      drivers/media/dvb/frontends/dib7000m.mod.o
  CC      drivers/media/dvb/frontends/dib7000p.mod.o
  CC      drivers/media/dvb/frontends/dib8000.mod.o
  CC      drivers/media/dvb/frontends/dib9000.mod.o
  CC      drivers/media/dvb/frontends/dibx000_common.mod.o
  CC      drivers/media/dvb/frontends/drxd.mod.o
  CC      drivers/media/dvb/frontends/drxk.mod.o
  CC      drivers/media/dvb/frontends/ds3000.mod.o
  CC      drivers/media/dvb/frontends/dvb-pll.mod.o
  CC      drivers/media/dvb/frontends/ec100.mod.o
  CC      drivers/media/dvb/frontends/hd29l2.mod.o
  CC      drivers/media/dvb/frontends/isl6405.mod.o
  CC      drivers/media/dvb/frontends/isl6421.mod.o
  CC      drivers/media/dvb/frontends/isl6423.mod.o
  CC      drivers/media/dvb/frontends/it913x-fe.mod.o
  CC      drivers/media/dvb/frontends/itd1000.mod.o
  CC      drivers/media/dvb/frontends/ix2505v.mod.o
  CC      drivers/media/dvb/frontends/lgdt3305.mod.o
  CC      drivers/media/dvb/frontends/l64781.mod.o
  CC      drivers/media/dvb/frontends/lgdt330x.mod.o
  CC      drivers/media/dvb/frontends/lgs8gl5.mod.o
  CC      drivers/media/dvb/frontends/lgs8gxx.mod.o
  CC      drivers/media/dvb/frontends/lnbp21.mod.o
  CC      drivers/media/dvb/frontends/lnbp22.mod.o
  CC      drivers/media/dvb/frontends/m88rs2000.mod.o
  CC      drivers/media/dvb/frontends/mb86a16.mod.o
  CC      drivers/media/dvb/frontends/mb86a20s.mod.o
  CC      drivers/media/dvb/frontends/mt312.mod.o
  CC      drivers/media/dvb/frontends/mt352.mod.o
  CC      drivers/media/dvb/frontends/nxt200x.mod.o
  CC      drivers/media/dvb/frontends/nxt6000.mod.o
  CC      drivers/media/dvb/frontends/or51132.mod.o
  CC      drivers/media/dvb/frontends/or51211.mod.o
  CC      drivers/media/dvb/frontends/s5h1409.mod.o
  CC      drivers/media/dvb/frontends/s5h1411.mod.o
  CC      drivers/media/dvb/frontends/s5h1420.mod.o
  CC      drivers/media/dvb/frontends/s5h1432.mod.o
  CC      drivers/media/dvb/frontends/s921.mod.o
  CC      drivers/media/dvb/frontends/si21xx.mod.o
  CC      drivers/media/dvb/frontends/sp8870.mod.o
  CC      drivers/media/dvb/frontends/sp887x.mod.o
  CC      drivers/media/dvb/frontends/stb0899.mod.o
  CC      drivers/media/dvb/frontends/stb6000.mod.o
  CC      drivers/media/dvb/frontends/stb6100.mod.o
  CC      drivers/media/dvb/frontends/stv0288.mod.o
  CC      drivers/media/dvb/frontends/stv0297.mod.o
  CC      drivers/media/dvb/frontends/stv0299.mod.o
  CC      drivers/media/dvb/frontends/stv0367.mod.o
  CC      drivers/media/dvb/frontends/stv0900.mod.o
  CC      drivers/media/dvb/frontends/stv090x.mod.o
  CC      drivers/media/dvb/frontends/stv6110.mod.o
  CC      drivers/media/dvb/frontends/stv6110x.mod.o
  CC      drivers/media/dvb/frontends/tda10021.mod.o
  CC      drivers/media/dvb/frontends/tda10023.mod.o
  CC      drivers/media/dvb/frontends/tda10048.mod.o
  CC      drivers/media/dvb/frontends/tda1004x.mod.o
  CC      drivers/media/dvb/frontends/tda10071.mod.o
  CC      drivers/media/dvb/frontends/tda18271c2dd.mod.o
  CC      drivers/media/dvb/frontends/tda10086.mod.o
  CC      drivers/media/dvb/frontends/tda665x.mod.o
  CC      drivers/media/dvb/frontends/tda8083.mod.o
  CC      drivers/media/dvb/frontends/tda8261.mod.o
  CC      drivers/media/dvb/frontends/tda826x.mod.o
  CC      drivers/media/dvb/frontends/ves1820.mod.o
  CC      drivers/media/dvb/frontends/tua6100.mod.o
  CC      drivers/media/dvb/frontends/ves1x93.mod.o
  CC      drivers/media/dvb/frontends/zl10036.mod.o
  CC      drivers/media/dvb/frontends/zl10039.mod.o
  CC      drivers/media/dvb/frontends/zl10353.mod.o
  CC      drivers/net/wireless/at76c50x-usb.mod.o
  CC      drivers/net/wireless/ath/ath6kl/ath6kl_usb.mod.o
  CC      drivers/net/wireless/ath/ath9k/ath9k.mod.o
  CC      drivers/net/wireless/ath/ath9k/ath9k_common.mod.o
  CC      drivers/net/wireless/ath/ath9k/ath9k_htc.mod.o
  CC      drivers/net/wireless/ath/ath9k/ath9k_hw.mod.o
  CC      drivers/net/wireless/ath/carl9170/carl9170.mod.o
  CC      drivers/net/wireless/rt2x00/rt2500usb.mod.o
  CC      drivers/net/wireless/rt2x00/rt2800lib.mod.o
  CC      drivers/net/wireless/rt2x00/rt2800usb.mod.o
  CC      drivers/net/wireless/rt2x00/rt2x00lib.mod.o
  CC      drivers/net/wireless/rt2x00/rt2x00usb.mod.o
  CC      drivers/net/wireless/rt2x00/rt73usb.mod.o
  CC      drivers/net/wireless/rtl818x/rtl8187/rtl8187.mod.o
  CC      drivers/net/wireless/rtlwifi/rtl8192c/rtl8192c-common.mod.o
  CC      drivers/net/wireless/rtlwifi/rtl8192cu/rtl8192cu.mod.o
  CC      drivers/net/wireless/rtlwifi/rtlwifi.mod.o
  CC      drivers/net/wireless/zd1201.mod.o
  CC      drivers/scsi/scsi_wait_scan.mod.o
  CC      lib/crc-itu-t.mod.o
  CC      net/mac80211/mac80211.mod.o
  LD [M]  drivers/bluetooth/bcm203x.ko
  LD [M]  drivers/bluetooth/bfusb.ko
  LD [M]  drivers/bluetooth/bpa10x.ko
  LD [M]  drivers/media/dvb/frontends/a8293.ko
  LD [M]  drivers/media/dvb/frontends/af9013.ko
  LD [M]  drivers/media/dvb/frontends/atbm8830.ko
  LD [M]  drivers/media/dvb/frontends/au8522.ko
  LD [M]  drivers/media/dvb/frontends/bcm3510.ko
  LD [M]  drivers/media/dvb/frontends/cx22700.ko
  LD [M]  drivers/media/dvb/frontends/cx22702.ko
  LD [M]  drivers/media/dvb/frontends/cx24110.ko
  LD [M]  drivers/media/dvb/frontends/cx24113.ko
  LD [M]  drivers/media/dvb/frontends/cx24116.ko
  LD [M]  drivers/media/dvb/frontends/cx24123.ko
  LD [M]  drivers/media/dvb/frontends/cxd2820r.ko
  LD [M]  drivers/media/dvb/frontends/dib0070.ko
  LD [M]  drivers/media/dvb/frontends/dib0090.ko
  LD [M]  drivers/media/dvb/frontends/dib3000mb.ko
  LD [M]  drivers/media/dvb/frontends/dib3000mc.ko
  LD [M]  drivers/media/dvb/frontends/dib7000m.ko
  LD [M]  drivers/media/dvb/frontends/dib7000p.ko
  LD [M]  drivers/media/dvb/frontends/dib8000.ko
  LD [M]  drivers/media/dvb/frontends/dib9000.ko
  LD [M]  drivers/media/dvb/frontends/dibx000_common.ko
  LD [M]  drivers/media/dvb/frontends/drxd.ko
  LD [M]  drivers/media/dvb/frontends/drxk.ko
  LD [M]  drivers/media/dvb/frontends/ds3000.ko
  LD [M]  drivers/media/dvb/frontends/ec100.ko
  LD [M]  drivers/media/dvb/frontends/dvb-pll.ko
  LD [M]  drivers/media/dvb/frontends/hd29l2.ko
  LD [M]  drivers/media/dvb/frontends/isl6405.ko
  LD [M]  drivers/media/dvb/frontends/isl6421.ko
  LD [M]  drivers/media/dvb/frontends/it913x-fe.ko
  LD [M]  drivers/media/dvb/frontends/isl6423.ko
  LD [M]  drivers/media/dvb/frontends/itd1000.ko
  LD [M]  drivers/media/dvb/frontends/ix2505v.ko
  LD [M]  drivers/media/dvb/frontends/l64781.ko
  LD [M]  drivers/media/dvb/frontends/lgdt3305.ko
  LD [M]  drivers/media/dvb/frontends/lgdt330x.ko
  LD [M]  drivers/media/dvb/frontends/lgs8gl5.ko
  LD [M]  drivers/media/dvb/frontends/lgs8gxx.ko
  LD [M]  drivers/media/dvb/frontends/lnbp21.ko
  LD [M]  drivers/media/dvb/frontends/lnbp22.ko
  LD [M]  drivers/media/dvb/frontends/m88rs2000.ko
  LD [M]  drivers/media/dvb/frontends/mb86a16.ko
  LD [M]  drivers/media/dvb/frontends/mb86a20s.ko
  LD [M]  drivers/media/dvb/frontends/mt312.ko
  LD [M]  drivers/media/dvb/frontends/mt352.ko
  LD [M]  drivers/media/dvb/frontends/nxt200x.ko
  LD [M]  drivers/media/dvb/frontends/nxt6000.ko
  LD [M]  drivers/media/dvb/frontends/or51132.ko
  LD [M]  drivers/media/dvb/frontends/or51211.ko
  LD [M]  drivers/media/dvb/frontends/s5h1409.ko
  LD [M]  drivers/media/dvb/frontends/s5h1411.ko
  LD [M]  drivers/media/dvb/frontends/s5h1420.ko
  LD [M]  drivers/media/dvb/frontends/s5h1432.ko
  LD [M]  drivers/media/dvb/frontends/s921.ko
  LD [M]  drivers/media/dvb/frontends/si21xx.ko
  LD [M]  drivers/media/dvb/frontends/sp8870.ko
  LD [M]  drivers/media/dvb/frontends/sp887x.ko
  LD [M]  drivers/media/dvb/frontends/stb0899.ko
  LD [M]  drivers/media/dvb/frontends/stb6000.ko
  LD [M]  drivers/media/dvb/frontends/stb6100.ko
  LD [M]  drivers/media/dvb/frontends/stv0288.ko
  LD [M]  drivers/media/dvb/frontends/stv0297.ko
  LD [M]  drivers/media/dvb/frontends/stv0299.ko
  LD [M]  drivers/media/dvb/frontends/stv0367.ko
  LD [M]  drivers/media/dvb/frontends/stv0900.ko
  LD [M]  drivers/media/dvb/frontends/stv090x.ko
  LD [M]  drivers/media/dvb/frontends/stv6110.ko
  LD [M]  drivers/media/dvb/frontends/stv6110x.ko
  LD [M]  drivers/media/dvb/frontends/tda10021.ko
  LD [M]  drivers/media/dvb/frontends/tda10048.ko
  LD [M]  drivers/media/dvb/frontends/tda10023.ko
  LD [M]  drivers/media/dvb/frontends/tda1004x.ko
  LD [M]  drivers/media/dvb/frontends/tda10071.ko
  LD [M]  drivers/media/dvb/frontends/tda10086.ko
  LD [M]  drivers/media/dvb/frontends/tda18271c2dd.ko
  LD [M]  drivers/media/dvb/frontends/tda665x.ko
  LD [M]  drivers/media/dvb/frontends/tda8083.ko
  LD [M]  drivers/media/dvb/frontends/tda8261.ko
  LD [M]  drivers/media/dvb/frontends/tda826x.ko
  LD [M]  drivers/media/dvb/frontends/tua6100.ko
  LD [M]  drivers/media/dvb/frontends/ves1820.ko
  LD [M]  drivers/media/dvb/frontends/ves1x93.ko
  LD [M]  drivers/media/dvb/frontends/zl10036.ko
  LD [M]  drivers/media/dvb/frontends/zl10039.ko
  LD [M]  drivers/media/dvb/frontends/zl10353.ko
  LD [M]  drivers/net/wireless/at76c50x-usb.ko
  LD [M]  drivers/net/wireless/ath/ath6kl/ath6kl_usb.ko
  LD [M]  drivers/net/wireless/ath/ath9k/ath9k.ko
  LD [M]  drivers/net/wireless/ath/ath9k/ath9k_common.ko
  LD [M]  drivers/net/wireless/ath/ath9k/ath9k_htc.ko
  LD [M]  drivers/net/wireless/ath/ath9k/ath9k_hw.ko
  LD [M]  drivers/net/wireless/ath/carl9170/carl9170.ko
  LD [M]  drivers/net/wireless/rt2x00/rt2500usb.ko
  LD [M]  drivers/net/wireless/rt2x00/rt2800lib.ko
  LD [M]  drivers/net/wireless/rt2x00/rt2800usb.ko
  LD [M]  drivers/net/wireless/rt2x00/rt2x00lib.ko
  LD [M]  drivers/net/wireless/rt2x00/rt2x00usb.ko
  LD [M]  drivers/net/wireless/rt2x00/rt73usb.ko
  LD [M]  drivers/net/wireless/rtl818x/rtl8187/rtl8187.ko
  LD [M]  drivers/net/wireless/rtlwifi/rtl8192c/rtl8192c-common.ko
  LD [M]  drivers/net/wireless/zd1201.ko
  LD [M]  drivers/scsi/scsi_wait_scan.ko
  LD [M]  drivers/net/wireless/rtlwifi/rtlwifi.ko
  LD [M]  lib/crc-itu-t.ko
  LD [M]  drivers/net/wireless/rtlwifi/rtl8192cu/rtl8192cu.ko
  LD [M]  net/mac80211/mac80211.ko
  AS      arch/arm/boot/compressed/piggy.xzkern.o
  LD      arch/arm/boot/compressed/vmlinux
  OBJCOPY arch/arm/boot/zImage
  Kernel: arch/arm/boot/zImage is ready
make: Leaving directory '/root/rerpie/kernel/google/msm'
Installing kernel modules to build/lib/modules...
make: Entering directory '/root/rerpie/kernel/google/msm'
  INSTALL drivers/bluetooth/bcm203x.ko
  INSTALL drivers/bluetooth/bfusb.ko
  INSTALL drivers/bluetooth/bpa10x.ko
  INSTALL drivers/media/dvb/frontends/a8293.ko
  INSTALL drivers/media/dvb/frontends/af9013.ko
  INSTALL drivers/media/dvb/frontends/atbm8830.ko
  INSTALL drivers/media/dvb/frontends/au8522.ko
  INSTALL drivers/media/dvb/frontends/bcm3510.ko
  INSTALL drivers/media/dvb/frontends/cx22700.ko
  INSTALL drivers/media/dvb/frontends/cx22702.ko
  INSTALL drivers/media/dvb/frontends/cx24110.ko
  INSTALL drivers/media/dvb/frontends/cx24113.ko
  INSTALL drivers/media/dvb/frontends/cx24116.ko
  INSTALL drivers/media/dvb/frontends/cx24123.ko
  INSTALL drivers/media/dvb/frontends/cxd2820r.ko
  INSTALL drivers/media/dvb/frontends/dib0070.ko
  INSTALL drivers/media/dvb/frontends/dib0090.ko
  INSTALL drivers/media/dvb/frontends/dib3000mb.ko
  INSTALL drivers/media/dvb/frontends/dib3000mc.ko
  INSTALL drivers/media/dvb/frontends/dib7000m.ko
  INSTALL drivers/media/dvb/frontends/dib7000p.ko
  INSTALL drivers/media/dvb/frontends/dib8000.ko
  INSTALL drivers/media/dvb/frontends/dib9000.ko
  INSTALL drivers/media/dvb/frontends/dibx000_common.ko
  INSTALL drivers/media/dvb/frontends/drxd.ko
  INSTALL drivers/media/dvb/frontends/drxk.ko
  INSTALL drivers/media/dvb/frontends/ds3000.ko
  INSTALL drivers/media/dvb/frontends/dvb-pll.ko
  INSTALL drivers/media/dvb/frontends/ec100.ko
  INSTALL drivers/media/dvb/frontends/hd29l2.ko
  INSTALL drivers/media/dvb/frontends/isl6405.ko
  INSTALL drivers/media/dvb/frontends/isl6421.ko
  INSTALL drivers/media/dvb/frontends/isl6423.ko
  INSTALL drivers/media/dvb/frontends/it913x-fe.ko
  INSTALL drivers/media/dvb/frontends/itd1000.ko
  INSTALL drivers/media/dvb/frontends/ix2505v.ko
  INSTALL drivers/media/dvb/frontends/l64781.ko
  INSTALL drivers/media/dvb/frontends/lgdt3305.ko
  INSTALL drivers/media/dvb/frontends/lgdt330x.ko
  INSTALL drivers/media/dvb/frontends/lgs8gl5.ko
  INSTALL drivers/media/dvb/frontends/lgs8gxx.ko
  INSTALL drivers/media/dvb/frontends/lnbp21.ko
  INSTALL drivers/media/dvb/frontends/lnbp22.ko
  INSTALL drivers/media/dvb/frontends/m88rs2000.ko
  INSTALL drivers/media/dvb/frontends/mb86a16.ko
  INSTALL drivers/media/dvb/frontends/mb86a20s.ko
  INSTALL drivers/media/dvb/frontends/mt312.ko
  INSTALL drivers/media/dvb/frontends/mt352.ko
  INSTALL drivers/media/dvb/frontends/nxt200x.ko
  INSTALL drivers/media/dvb/frontends/nxt6000.ko
  INSTALL drivers/media/dvb/frontends/or51132.ko
  INSTALL drivers/media/dvb/frontends/or51211.ko
  INSTALL drivers/media/dvb/frontends/s5h1409.ko
  INSTALL drivers/media/dvb/frontends/s5h1411.ko
  INSTALL drivers/media/dvb/frontends/s5h1420.ko
  INSTALL drivers/media/dvb/frontends/s5h1432.ko
  INSTALL drivers/media/dvb/frontends/s921.ko
  INSTALL drivers/media/dvb/frontends/si21xx.ko
  INSTALL drivers/media/dvb/frontends/sp8870.ko
  INSTALL drivers/media/dvb/frontends/sp887x.ko
  INSTALL drivers/media/dvb/frontends/stb0899.ko
  INSTALL drivers/media/dvb/frontends/stb6000.ko
  INSTALL drivers/media/dvb/frontends/stb6100.ko
  INSTALL drivers/media/dvb/frontends/stv0288.ko
  INSTALL drivers/media/dvb/frontends/stv0297.ko
  INSTALL drivers/media/dvb/frontends/stv0299.ko
  INSTALL drivers/media/dvb/frontends/stv0367.ko
  INSTALL drivers/media/dvb/frontends/stv0900.ko
  INSTALL drivers/media/dvb/frontends/stv090x.ko
  INSTALL drivers/media/dvb/frontends/stv6110.ko
  INSTALL drivers/media/dvb/frontends/stv6110x.ko
  INSTALL drivers/media/dvb/frontends/tda10021.ko
  INSTALL drivers/media/dvb/frontends/tda10023.ko
  INSTALL drivers/media/dvb/frontends/tda10048.ko
  INSTALL drivers/media/dvb/frontends/tda1004x.ko
  INSTALL drivers/media/dvb/frontends/tda10071.ko
  INSTALL drivers/media/dvb/frontends/tda10086.ko
  INSTALL drivers/media/dvb/frontends/tda18271c2dd.ko
  INSTALL drivers/media/dvb/frontends/tda665x.ko
  INSTALL drivers/media/dvb/frontends/tda8083.ko
  INSTALL drivers/media/dvb/frontends/tda8261.ko
  INSTALL drivers/media/dvb/frontends/tda826x.ko
  INSTALL drivers/media/dvb/frontends/tua6100.ko
  INSTALL drivers/media/dvb/frontends/ves1820.ko
  INSTALL drivers/media/dvb/frontends/ves1x93.ko
  INSTALL drivers/media/dvb/frontends/zl10036.ko
  INSTALL drivers/media/dvb/frontends/zl10039.ko
  INSTALL drivers/media/dvb/frontends/zl10353.ko
  INSTALL drivers/net/wireless/at76c50x-usb.ko
  INSTALL drivers/net/wireless/ath/ath6kl/ath6kl_usb.ko
  INSTALL drivers/net/wireless/ath/ath9k/ath9k.ko
  INSTALL drivers/net/wireless/ath/ath9k/ath9k_common.ko
  INSTALL drivers/net/wireless/ath/ath9k/ath9k_htc.ko
  INSTALL drivers/net/wireless/ath/ath9k/ath9k_hw.ko
  INSTALL drivers/net/wireless/ath/carl9170/carl9170.ko
  INSTALL drivers/net/wireless/rt2x00/rt2500usb.ko
  INSTALL drivers/net/wireless/rt2x00/rt2800lib.ko
  INSTALL drivers/net/wireless/rt2x00/rt2800usb.ko
  INSTALL drivers/net/wireless/rt2x00/rt2x00lib.ko
  INSTALL drivers/net/wireless/rt2x00/rt2x00usb.ko
  INSTALL drivers/net/wireless/rt2x00/rt73usb.ko
  INSTALL drivers/net/wireless/rtl818x/rtl8187/rtl8187.ko
  INSTALL drivers/net/wireless/rtlwifi/rtl8192c/rtl8192c-common.ko
  INSTALL drivers/net/wireless/rtlwifi/rtl8192cu/rtl8192cu.ko
  INSTALL drivers/net/wireless/rtlwifi/rtlwifi.ko
  INSTALL drivers/net/wireless/zd1201.ko
  INSTALL drivers/scsi/scsi_wait_scan.ko
  INSTALL lib/crc-itu-t.ko
  INSTALL net/mac80211/mac80211.ko
  DEPMOD  3.4.113-Kali-0E800.nethunter-flo-1.0-g5452e51bb642
make: Leaving directory '/root/rerpie/kernel/google/msm'
Finished building nethunter-flo-1.0!
```
