# 2011-06-10: File changed by Sony Corporation
obj-y                                   += common.o
obj-y                                   += apbio.o
obj-y                                   += io.o
obj-y                                   += irq.o legacy_irq.o
obj-y                                   += syncpt.o
obj-y                                   += clock.o
obj-y                                   += dvfs.o
obj-y                                   += timer.o
obj-y                                   += gpio.o
obj-y                                   += pinmux.o
obj-y                                   += devices.o
obj-y                                   += delay.o
obj-y                                   += powergate.o
obj-y                                   += suspend.o
obj-y                                   += fuse.o
obj-y                                   += kfuse.o
ifeq ($(CONFIG_TEGRA_ALSA),y)
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)         += tegra2_i2s.o
else
obj-y                                   += tegra_i2s_audio.o
obj-y                                   += tegra_spdif_audio.o
endif
obj-y                                   += spdif.o
obj-y                                   += tegra_das.o
obj-y                                   += mc.o
obj-$(CONFIG_USB_SUPPORT)               += usb_phy.o
obj-$(CONFIG_FIQ)                       += fiq.o
obj-$(CONFIG_TEGRA_FIQ_DEBUGGER)        += tegra_fiq_debugger.o
obj-$(CONFIG_TEGRA_PWM)                 += pwm.o
obj-$(CONFIG_TEGRA_ARB_SEMAPHORE)	+= arb_sema.o

obj-$(CONFIG_ARCH_TEGRA_2x_SOC)         += clock.o
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)         += tegra2_clocks.o
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)         += tegra2_dvfs.o
ccflags-${CONFIG_MACH_NBX02} += -DNBX_WORKAROUND_DVFS_AP20H_VOLTABLE
ccflags-${CONFIG_MACH_NBX03} += -DNBX_WORKAROUND_DVFS_AP20H_VOLTABLE
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)         += tegra2_fuse.o
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)         += tegra2_speedo.o
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)         += suspend-t2.o
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)		+= tegra2_save.o
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)		+= tegra2_emc.o
obj-$(CONFIG_CPU_V7)			+= cortex-a9.o

obj-$(CONFIG_ARCH_TEGRA_2x_SOC)		+= pinmux-t2-tables.o
obj-$(CONFIG_SMP)                       += localtimer.o
obj-$(CONFIG_SMP)                       += platsmp.o
obj-y                                   += headsmp.o
obj-$(CONFIG_ARCH_TEGRA_2x_SOC)         += headsmp-t2.o
obj-$(CONFIG_TEGRA_SYSTEM_DMA)          += dma.o
obj-$(CONFIG_CPU_FREQ)                  += cpu-tegra.o
obj-$(CONFIG_CPU_IDLE)                  += cpuidle.o
obj-$(CONFIG_TEGRA_IOVMM)               += iovmm.o
obj-$(CONFIG_TEGRA_IOVMM_GART)          += iovmm-gart.o
obj-$(CONFIG_TEGRA_MC_PROFILE)          += tegra2_mc.o

obj-y                                   += nv/

obj-${CONFIG_TEGRA_SPI_SLAVE}		+= spi_tegra_slave.o

obj-${CONFIG_MACH_HARMONY}              += board-harmony.o
obj-${CONFIG_MACH_HARMONY}              += board-harmony-pinmux.o
obj-${CONFIG_MACH_HARMONY}              += board-harmony-panel.o
obj-${CONFIG_MACH_HARMONY}              += board-harmony-sdhci.o

obj-${CONFIG_MACH_VENTANA}              += board-ventana.o
obj-${CONFIG_MACH_VENTANA}              += board-ventana-pinmux.o
obj-${CONFIG_MACH_VENTANA}              += board-ventana-sdhci.o
obj-${CONFIG_MACH_VENTANA}              += board-ventana-power.o
obj-${CONFIG_MACH_VENTANA}              += board-ventana-panel.o
obj-${CONFIG_MACH_VENTANA}              += board-ventana-jack.o
obj-${CONFIG_MACH_VENTANA}              += board-ventana-sensors.o
obj-${CONFIG_MACH_VENTANA}              += board-ventana-kbc.o
obj-${CONFIG_MACH_VENTANA}              += board-ventana-memory.o

obj-${CONFIG_MACH_WHISTLER}             += board-whistler.o
obj-${CONFIG_MACH_WHISTLER}             += board-whistler-pinmux.o
obj-${CONFIG_MACH_WHISTLER}             += board-whistler-sdhci.o
obj-${CONFIG_MACH_WHISTLER}             += board-whistler-power.o
obj-${CONFIG_MACH_WHISTLER}             += board-whistler-panel.o
obj-${CONFIG_MACH_WHISTLER}             += board-whistler-sensors.o
obj-${CONFIG_MACH_WHISTLER}             += board-whistler-kbc.o
obj-${CONFIG_MACH_WHISTLER}             += board-whistler-baseband.o
obj-${CONFIG_MACH_WHISTLER}             += board-whistler-memory.o

obj-${CONFIG_MACH_NBX02}                += board-nbx02.o
obj-${CONFIG_MACH_NBX02}                += board-nbx02-pinmux.o
obj-${CONFIG_MACH_NBX02}                += board-nbx02-sdhci.o
obj-${CONFIG_MACH_NBX02}                += board-nbx02-power.o
obj-${CONFIG_MACH_NBX02}                += board-nbx02-panel.o
obj-${CONFIG_MACH_NBX02}                += board-nbx02-sensors.o
obj-${CONFIG_MACH_NBX02}                += board-nbx02-kbc.o
obj-${CONFIG_MACH_NBX02}                += board-nbx02-memory.o
obj-${CONFIG_MACH_NBX02}                += board-nbx02-jack.o
obj-${CONFIG_MACH_NBX02}                += wireless_power_control_nbx02.o
obj-${CONFIG_MACH_NBX02}                += sysfs-wirelesspower.o
obj-${CONFIG_MACH_NBX02}                += board-nbx-common.o
obj-${CONFIG_MACH_NBX02}                += a1026.o
ccflags-${CONFIG_MACH_NBX02} += -DNBX_SET_SDIO1_MAXCLK_26MHZ

obj-${CONFIG_MACH_NBX03}                += board-nbx03.o
obj-${CONFIG_MACH_NBX03}                += board-nbx03-pinmux.o
obj-${CONFIG_MACH_NBX03}                += board-nbx03-sdhci.o
obj-${CONFIG_MACH_NBX03}                += board-nbx03-power.o
obj-${CONFIG_MACH_NBX03}                += board-nbx03-panel.o
obj-${CONFIG_MACH_NBX03}                += board-nbx03-sensors.o
obj-${CONFIG_MACH_NBX03}                += board-nbx03-kbc.o
obj-${CONFIG_MACH_NBX03}                += board-nbx03-jack.o
obj-${CONFIG_MACH_NBX03}                += board-nbx03-memory.o
obj-${CONFIG_MACH_NBX03}                += wireless_power_control_nbx03.o
obj-${CONFIG_MACH_NBX03}                += sysfs-wirelesspower.o
obj-${CONFIG_MACH_NBX03}                += hci-event.o
obj-${CONFIG_MACH_NBX03}                += board-nbx-common.o
obj-${CONFIG_MACH_NBX03}                += a1026.o
ccflags-${CONFIG_MACH_NBX03} += -DNBX_SET_SDIO1_MAXCLK_26MHZ
