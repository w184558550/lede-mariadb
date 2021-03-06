[//]: #@corifeus-header

## The LEDE Stable MariaDB 5.5.58 package

---
                        
[//]: #@corifeus-header:end
# Create package

```bash
rm build_dir/target-arm_cortex-a9+vfpv3_musl-1.1.16_eabi/mariadb* -rf
rm build_dir/target-mipsel_24kc_musl-1.1.16/mariadb* -rf
rm feeds/mariadb* -rf
./scripts/feeds update -a
./scripts/feeds install -a

# once you already updated the all
./scripts/feeds install mariadb
./scripts/feeds update -a -p mariadb

make package/feeds/mariadb/mariadb/{clean,prepare,compile} package/index V=s
```
[//]: #@corifeus-footer

---

[**P3X-LEDE-MARIADB**](https://pages.corifeus.com/lede-mariadb) Build v5.5.154-176 

[![Like Corifeus @ Facebook](https://img.shields.io/badge/LIKE-Corifeus-3b5998.svg)](https://www.facebook.com/corifeus.software) [![Donate for Corifeus / P3X](https://img.shields.io/badge/Donate-Corifeus-003087.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=QZVM4V6HVZJW6)  [![Contact Corifeus / P3X](https://img.shields.io/badge/Contact-P3X-ff9900.svg)](https://www.patrikx3.com/en/front/contact) 


## Sponsor

[![JetBrains](https://www.patrikx3.com/images/jetbrains-logo.svg)](https://www.jetbrains.com/)
  
 

[//]: #@corifeus-footer:end