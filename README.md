# 角色画师管理器 (V3.4)

一个用于管理、浏览和使用AI绘画角色提示词（Prompt）的在线工具。

**[➡️ 在线体验 (Live Demo)](https://970224023.github.io/anime-character-manager/)**

---

## 关于开发

你好！这个项目由我构思，并由Google的Gemini Pro模型完成全部代码实现。作为一个AI绘画爱好者，我发现在使用NovelAI时，从海量的角色中寻找、挑选并正确输入角色与作品名是一个非常繁琐的过程。为了解决这个痛点，我创造了这个管理器，希望能让你轻松地浏览角色库，只需轻轻一点，就能获得准确、好用的Prompt。

## 主要功能

本工具经过多次迭代，已具备一套完整、高效的管理与使用流程：

-   **分类管理与浏览**: 自动根据作品（出处）对角色进行分组，左侧列表一目了然。
    ![快速查找作品](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/06_category_index.jpg)

-   **详情速览**: 单击任意角色卡片，即可在右侧详情栏查看其高清大图、人物简介、属性标签等信息。
    ![角色详细信息](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/04_detail_panel.jpg)

-   **便捷的Prompt复制**: **再次单击已选中的卡片**，或点击详情栏的【复制Prompt】按钮，即可快速复制优化后的AI绘画提示词。
    ![复制角色Prompt](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/03_character_card.jpg)

-   **图文双视图**: 可在紧凑的**文字列表**和直观的**图片画廊**模式之间自由切换，满足不同浏览习惯。（注：为保证流畅，图文模式仅在单个作品分类下生效）
    ![图文切换与编辑模式](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/07_view_modes.jpg)

-   **Prompt微调工具**: 详情栏提供了【调换】按钮，可一键调换Prompt中姓与名的顺序，以应对部分角色因姓名顺序错误而无法被AI识别的问题。

-   **安全编辑模式**: 提供全局【编辑】开关。开启后，界面背景会变为护眼的绿色以作提示，此时单击卡片将直接进入编辑界面，有效防止误操作。
    ![编辑角色界面](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/05_edit_modal.jpg)
    
-   **随机选择**: 不知道想画谁？点击右上角的【🎲】按钮，让命运为你挑选下一位角色！
    ![随机选择角色](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/09_random_select.jpg)

-   **灵活的数据操作**: 支持从本地加载和保存`.json`格式的数据。加载时可选择【合并】或【覆盖】现有数据，方便你管理自己的角色库。
    ![加载与合并数据](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/02_merge_or_overwrite.jpg)

-   **添加与批量导入**: 支持手动【添加】单个角色，也保留了【批量导入】功能。
    > **说明**: 【批量导入】功能需要配合一套特定格式的文本，主要是我个人用于快速补充数据的工具流，普通用户通常无需使用。
    ![添加与批量导入](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/08_batch_import.jpg)

## 如何使用

在线版已预先加载了默认数据，开箱即用。你也可以通过以下步骤管理自己的本地数据：

1.  **加载数据**:
    - 点击管理器右上角的【加载】按钮，选择你自己的 `.json` 角色数据文件。
    - 你可以使用仓库中提供的 `default_data.json` 作为模板来创建或扩充你的数据库。
    ![加载数据](https://raw.githubusercontent.com/970224023/anime-character-manager/main/screenshots/01_load_button.jpg)

2.  **浏览与操作**:
    - **查找**: 在左侧选择作品分类，或点击顶部的【品】字形按钮，通过A-Z索引快速定位作品。
    - **查看**: 在中栏浏览角色卡片，**单击**卡片在右侧查看详情。
    - **复制**: **再次单击**已选中的卡片，即可复制Prompt。

3.  **保存数据**:
    - 在进行任何添加、修改或删除操作后，请务必点击右上角的【保存】按钮。
    - 这会将你当前的所有数据（包括默认数据和你自己加载的数据）整合后，下载为一个新的 `manager_data.json` 文件，以便下次使用。

## 开源许可证

本项目采用 [MIT License](./LICENSE) 开源。

## 致谢

- 数据来源于 [MyAnimeList (MAL)](https://myanimelist.net/)。
- 通过优秀的社区项目 [Jikan API](https://jikan.moe/) 获取。

请尊重并合理使用以上服务。
