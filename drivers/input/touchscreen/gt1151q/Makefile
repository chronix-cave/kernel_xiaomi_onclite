#
# Makefile for the goodix touchscreen drivers.
#
obj-$(CONFIG_TOUCHSCREEN_GX)	+=  gt1x_extents.o
obj-$(CONFIG_TOUCHSCREEN_GX)	+=  gt1x_generic.o
obj-$(CONFIG_TOUCHSCREEN_GX)	+=  gt1x_tools.o
obj-$(CONFIG_TOUCHSCREEN_GX)	+=  gt1x.o
obj-$(CONFIG_TOUCHSCREEN_GX)	+=  gt1x_update.o
obj-$(CONFIG_TOUCHSCREEN_GX)    +=  gt1x_test.o
obj-$(CONFIG_TOUCHSCREEN_GX)    +=  test_function.o

# test_function.o provides its own fwrite(); keep the compiler from
# rewriting it into the libc fwrite_unlocked() builtin.
CFLAGS_test_function.o := -fno-builtin
