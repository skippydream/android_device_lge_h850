# android_device_lge_h850
h850 PARTITION_SIZE values are different from other LG G5s ones: cannot retrive them from g5-common.
WARNING: for that reason g5-common/BoardConfig.mk won't contain anymore #Partitions values, which have to be added in device/lge/*your-specific-lgg5-device*/BoardConfig.mk like this:
# Partitions
BOARD_BOOTIMAGE_PARTITION_SIZE := xxxxxxxx
BOARD_CACHEIMAGE_PARTITION_SIZE := 
BOARD_PERSISTIMAGE_PARTITION_SIZE := 
BOARD_RECOVERYIMAGE_PARTITION_SIZE := 
BOARD_SYSTEMIMAGE_PARTITION_SIZE := 
BOARD_USERDATAIMAGE_PARTITION_SIZE :=
