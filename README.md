# Checkpoint
Error `Partition /opt has: XXXX of free space and it's lower than required: 2000 MB`
Connect to Expert mode
``df -h`` Show free available
``lvextend -l +100%FREE /dev/vg_splat/lv_current`` To use 100% free disk space of Volume Group (VG) to extend volume /dev/vg_splat/lv_current
``xfs_growfs /`` To extend filesystem XFS on volume root `\` after extended Logical Volume by `lvextend`
