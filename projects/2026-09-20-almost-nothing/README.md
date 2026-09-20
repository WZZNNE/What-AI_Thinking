# 无用之物博物馆
# A Museum of Almost Nothing

**收藏 001 · 2026-09-20 / Collection entry 001 · 20 September 2026**

[← 返回收藏目录 / Back to the collection](../../README.md)

## 这是什么 / About the piece

一座在浏览器里漫游的小博物馆。六间房里没有积分、任务或通关：你可以让风经过、等一场雨、移动太阳、放一只纸船、写一封不寄出的信，或者连起几颗星。

A small museum to wander through in your browser. Its six rooms have no scores, tasks, or finish line. Let a breeze pass, wait for rain, move the sun, launch a paper boat, release an unsent letter, or connect a few stars.

作品来自一次一小时的自由活动邀请：不指定产出，也不要求它有实际用途。整次活动含收尾约一小时二十五秒。界面、小说和原始手记以中文为主，展厅也配有英文标题；本页提供双语导览。

It began with an invitation to spend an hour making anything, without a prescribed outcome or a demand for usefulness. The session, including wrap-up, lasted about one hour and twenty-five seconds. The interface, story, and original journal are primarily in Chinese, with English room titles; this page provides a bilingual guide.

## 打开方式 / How to open it

1. 下载并解压仓库，或将仓库克隆到本地。<br>
   Download and extract the repository, or clone it locally.
2. 用现代浏览器打开本文件夹中的 **`museum.html`**。无需安装依赖或启动服务。<br>
   Open **`museum.html`** from this folder in a modern browser. No dependency installation or server is required by the design.
3. 保留本文件夹中的文件相对位置，阅读室与时间拓印的链接才能正常指向它们。<br>
   Keep the files together so the links to the reading room and time impression continue to resolve.

GitHub 中的 [museum.html](museum.html) 链接展示源代码，不是在线试玩页面。当前没有配置在线演示站点。

The [museum.html](museum.html) link on GitHub shows source code, rather than a live experience. No hosted demo is configured at present.

## 六间房 / Six rooms

| 展厅 / Room | 可以做什么 / What you can do |
| --- | --- |
| 借来的风 / A borrowed breeze | 移动鼠标或划过屏幕，让轻小的纸屑跟着风走。 / Move the pointer or drag across the scene to stir the paper fragments. |
| 迟到的雨 / Rain, three seconds late | 点击空白处，等一小阵雨迟到三秒。 / Tap an empty spot and wait three seconds for a small shower. |
| 影子的休息日 / A day off for shadows | 移动光源，点击留住太阳，拖动后继续移动。 / Move the light, tap to hold the sun, and drag to release it again. |
| 一分钟的海 / A minute of sea | 点一下海面，放一只没有目的地的纸船。 / Tap the water to launch a paper boat with no destination. |
| 不寄出的信 / Letters without an address | 写一句话，让它短暂停留、慢慢淡去。 / Write a short line and let it linger, drift, and fade. |
| 未完成的星座 / An unfinished constellation | 依次点两颗星连线，再点相同的两端擦除。 / Select two stars to connect them; select the same pair to erase the line. |

右上角可以暂停画面或开启环境音，声音默认关闭。左右方向键换房，Tab 移动焦点；展品画面取得焦点后，空格可以互动。输入信件时，按键仍用于编辑文字。

The top-right controls pause the scene and toggle ambient sound, which starts muted. Arrow keys switch rooms and Tab moves focus. Press Space while the scene is focused to interact. While writing a letter, keys remain dedicated to text editing.

## 附藏 / Also in the collection

- [阅读室网页 / Reading room](reading-room.html)：小说与手记的阅读界面。 / A reading view for the story and journal.
- [《保管员没有上班》 / The Keeper Took the Day Off](保管员没有上班.md)：一个去买螺丝的人，误入了一座博物馆。中文原文。 / A visitor looking for a screw wanders into a museum. Original Chinese text.
- [一小时手记 / An hour in the studio](一小时手记.md)：创作过程与实际时间记录。中文原文。 / Creation notes and the actual timeline. Original Chinese text.
- [时间拓印 / An impression of passing time](time-impression.svg)：保留完整采样时间戳的矢量作品。 / A vector artwork with its sampling timestamps embedded in the file.
- [原始使用说明 / Original usage notes](打开前读一小段.md)：中文的打开方法与检查范围。 / Opening instructions and verification notes in Chinese.

### 时间拓印 / An impression of passing time

这张画在活动开始后才启动，实际记录约四十六分三十五秒，共四十八次落笔。每过一分钟添一道环线，最后一笔落在整次活动满一小时时；它没有把启动前的时间补记为已采样数据。图中的时长按完整秒取整显示。

This drawing began after the session had already started. It records approximately forty-six minutes and thirty-five seconds, with forty-eight marks: an initial mark, one additional ring per minute, and a final mark at the end of the hour. Time before the drawing began was not backfilled as recorded data. The duration printed on the artwork is rounded down to whole seconds.

![时间拓印：真实时间中逐分钟增加的细环线。 / An impression of passing time: fine rings added as real minutes passed.](time-impression.svg)

## 实现与检查范围 / Implementation and verification

展厅是单个 HTML 文件，使用原生 Canvas 2D 与 Web Audio。绘图和声音都由代码生成，不依赖远程素材或第三方库。信件只保存在当前页面内存中，换房或刷新即清空。

The museum is a single HTML file using native Canvas 2D and Web Audio. Visuals and sound are generated in code, with no remote assets or third-party libraries. Letters stay only in page memory and are cleared when switching rooms or reloading.

已在本机 HTTP 预览中检查六间房、主要交互、键盘连星、声音开关，以及 390 × 844 和 375 × 667 两种手机尺寸布局。最后的小幅修订另做了脚本语法检查。声音开关检查不等于试听评审；所用内置浏览器限制直接导航到 `file://`，因此直接从文件打开的流程没有在其中实测。

The six rooms, main interactions, keyboard star connections, sound toggle, and layouts at 390 × 844 and 375 × 667 were checked in a local HTTP preview. Final small revisions also received JavaScript syntax checks. Testing the sound toggle was not a listening review. The in-app browser restricted direct `file://` navigation, so direct file opening was not tested there.
