# alientek-imx6u-alpha

## u-boot patch
```shell
git clone https://github.com/nxp-imx/uboot-imx.git uboot-imx-rel_imx_4.1.15_2.1.0_ga --depth=1 -b rel_imx_4.1.15_2.1.0_ga
cd ~/linux/imx6ull/uboot/uboot-imx-rel_imx_4.1.15_2.1.0_ga
# Create / apply uboot patch.
git diff rel_imx_4.1.15_2.1.0_ga > ~/github/alientek-imx6u-alpha/patch/uboot-imx-rel_imx_4.1.15_2.1.0_ga_alientek.patch

patch -p1 < ~/github/alientek-imx6u-alpha/patch/uboot-imx-rel_imx_4.1.15_2.1.0_ga_alientek.patch

```