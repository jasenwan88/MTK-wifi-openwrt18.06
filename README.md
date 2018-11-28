# mtk wifi driver for openwrt 18.06(linux-4.14.68)
# mt7620-p4rev-120998.tar.bz2 in mtk-openwrt SDK
# The following specific migration steps:
	
	1, mv mt7620-p4rev-120998.tar.bz2 openwrt/dl/
	2, mv mtk-wfi-openwrt18.06  openwrt/packages/ramips
	3, make menuconfig->MTK Properties
	4, make V=s

