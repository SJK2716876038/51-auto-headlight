# firmware 程序清单

课设的程序是 STC89C52 的 Keil C51 工程，按功能拆成了几个源文件：

| 文件 | 作用 |
| --- | --- |
| main.c | 主循环与工作模式状态机，Timer0 定时 1ms 提供任务节拍 |
| Key.c | 按键扫描与消抖 |
| Seg.c | 数码管动态扫描与多界面显示 |
| Oled.c | OLED 显示驱动 |
| Adc.c | 光强采样 |

原始 Keil 工程在当年做课设的电脑上，暂未整理进来；课程设计说明书里附有 main.c 的完整程序清单。

提交时不要带 Objects/、Listings/ 和 *.o、*.lst、*.m51 这些编译产物，已在 .gitignore 里排除。
