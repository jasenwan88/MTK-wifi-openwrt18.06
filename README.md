# mtk wifi driver for openwrt 18.06(linux-4.14.68)
# The following specific migration steps:
	
	1, mv mtk-wfi-openwrt18.06  packages/ramips
	2, make menuconfig->MTK Properties
	3, make V=s

