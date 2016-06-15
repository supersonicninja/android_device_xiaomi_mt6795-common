# CM12.1 Device tree for Redmi Note 2 (HERMES)

### Other resource:
  - Kernel source: Not released yet
  - Vendor blobs: https://github.com/jianminglok/android_vendor_xiaomi_hermes

### Credits (Sort by alphabetical order):
  - jianminglok
  - lbule
  - nofearnohappy
  - Syl191 for the patches
  - The CyanogenMod Team
  - xen0n
  - xiaomi-dev (ivan19871002)


#### You have to revert some commits for selinux ioctl(policyver30)
cd external/selinux
git revert 7c912dbc7c926629474387f39f9b86cf94477cd7
git revert 80bc7ee8faaddfa7a650994fa82a57f41a9e7475

cd externel/sepolicy
git revert 4b4b2b92939cd25095e247d0ed78f600fe40036d 
git revert de9b5301a14abf388589b06e819bb001d69e0cf1 (manual)
git revert a0fbeb97c0476891e177fb04953367aae90fc8a9
git revert 86f30cb16a8aa2ea337b1c36071bfa833f798c96 (manual)
git revert e0c8da253c8135e72bd84729d44e6b254d83f64b (manual)
