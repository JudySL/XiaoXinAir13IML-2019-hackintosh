# 热补丁
| 补丁                      | 说明                        | 必备 | 建议 | 可选 |
| ------------------------- | --------------------------- | ---- | ---- | ---- |
| SSDT-GPRW                 | 0D/6D睡了即醒补丁           |      | ✅    |      |
| SSDT-EC-USBX-air13iml     | EC+USBX                     | ✅    |      |      |
| SSDT-PNLF-CFL             | 亮度控制补丁                | ✅    |      |      |
| SSDT-MCHC                 | 仿冒MCHC设备                |      |      | ✅    |
| SSDT-LPAD-air13iml        | I2C触控板补丁               | ✅    |      |      |
| SSDT-PMCR                 | 仿冒PMC设备                 | ✅    |      |      |
| SSDT-RMCF-PS@Map-air13iml | PS2按键映射补丁             |      | ✅    |      |
| SSDT-PR00                 | CPU电源管理补丁（开启XCPM） | ✅    |      |      |
| SSDT-OCGPI0-GPHD          | OCI2C-GPIO补丁              |      | ✅    |      |
| SSDT-RTC_Y-AWAC_N         | 启用 RTC 并同时禁用 AWAC    |      | ✅    |      |
| SSDT-BATS-Air14IML        | 电池附加信息                |      |      | ✅    |
| SSDT-DMAC                 | 仿冒DMA控制器               |      |      | ✅    |

* 必备 : 影响各个部件的功能使用 , 开启
* 建议 : 兼容性补丁 , 非必要 , 建议开启
* 可选 : 只是一种完善方案 , 非必要 , 默认关闭 , 可自行选择是否开启
* 展开学习可参考<b>宪武</b> 提供的 [OC-little](https://github.com/daliansky/OC-little)和[<b>Dortania</b>](https://dortania.github.io/)的[Getting Started With ACPI](https://dortania.github.io/Getting-Started-With-ACPI/)
