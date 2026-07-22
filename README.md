# Introduction
Script version of [Official Bazzite guidance](https://docs.bazzite.gg/Advanced/swapfile/) to make enabling Hibernate easier.
Work of [Vudu](https://github.com/crnisamuraj).

# Methodology
- Automatically calculate ideal swap size
- Use BTRFS to create a NoCOW swapfile in a subvolume
- Set swappiness to 0
- Compile SELinux policy to fix "Access Denied" errors
- Update `rpm-ostree kargs` with resume UUID and offset
- Enable additional Suspend-then-Hibernate behaviour for extra responsiveness

# How to install
1. Git clone https://github.com/crnisamuraj/enable-bazzite-hibernate
2. Run bazzite-hibernate.sh as root
3. Restart machine

# Disclaimer
Software is provided as-is and places your Bazzite system in a state that is not supported by the script developers or Bazzite developers. Your Mileage May Vary.
