# my-awesome-copilot
好用的Github Copilot資源與Prompt


# 說明
- 身為github copilot使用者，定期去看看[Awesome Copilot](https://github.com/github/awesome-copilot?tab=readme-ov-file#-custom-chat-modes)有沒有什麼好東西是必要的。
- 這個repo主要是我在使用Github Copilot的過程中，覺得好用的資源與Prompt
- 有些設定是參考網友的分享，自己修改後覺得不錯的!


<br><br>

# 基本設定

推薦Will保哥的 [最佳 GitHub Copilot 設定](https://github.com/doggy8088/github-copilot-configs)，裡面有講解詳細的設定內容

設定檔 : [settings.json](.vscode/settings.json)

<br><br>

# MCP

## Figma
- [GitHub Copilot + Figma MCP Server 實戰：用 AI 快速切版教學](https://www.letswrite.tw/github-copilot-figma-mcp/)
- 作者將安裝步驟寫得很清楚，照著做就好




<br><br>

# [chatmodes](https://github.com/github/awesome-copilot?tab=readme-ov-file#-custom-chat-modes)

## [4.1-Beast.chatmode.md](https://github.com/github/awesome-copilot/blob/main/chatmodes/4.1-Beast.chatmode.md)

**野獸模式，覺得這個必設定的**，可以讓你的Copilot更聰明。但我看原作者Gist底下的討論，似乎有些小瑕疵，例如:
  - 使用Google搜尋可能會被Goole的反爬蟲檔掉，所以有人修改成使用Bing搜尋
  - 無法像Agent一樣自動寫入檔案，解法就是加編輯檔案指令到.md中

附上綜合網友建議後的修改版本：[4.1-Beast.chatmode.md](chatmodes/4.1-Beast.chatmode.md)

影片教學 : [解鎖 GitHub Copilot 野獸模式 | 教你自訂 Chat Mode 提升 AI 代理實力](https://www.youtube.com/watch?v=cK8HOfGEx24&t=9s)


<br><br>

# [prompts](https://github.com/github/awesome-copilot?tab=readme-ov-file#-reusable-prompts)

## Kiro工作流的三指令
- 這個prompt其實是我參考[🚀Claude Code重磅推出Sub agents功能！轻松实现任务专业化和模块化！三分钟完美复现Kiro工作流，规范驱动开发时代正式到来！从Vibe Coding到spec-driven软件开发！](https://www.youtube.com/watch?v=GjlkRcNNONo&ab_channel=AI%E8%B6%85%E5%85%83%E5%9F%9F)修改來的設定，原作者是在Claude Code中，使用Sub Agent達到像Kiro那樣的Spec-driven的開發方式。
- 不囉嗦!直接附上設定檔 : 
    - [kiro-01-steering-architect.prompt.md](prompts/kiro-01-steering-architect.prompt.md)
    - [kiro-02-strategic-planner.prompt.md](prompts/kiro-02-strategic-planner.prompt.md)
    - [kiro-03-task-executor.prompt.md](prompts/kiro-03-task-executor.prompt.md)
- 我自己試驗還是在Claude Code效果比較好，但為了在Github Copilot有一樣工作流，所以我修改了這些prompt，讓它們可以在Github Copilot中使用。
- 大家可以根據自己的需求修改
- 使用方式 : 
```bash
1. /steering-architect 幫我創建一個todo list的專案文件，技術使用html+css+Javascript


2. /strategic-planner 規劃todo list(HTML+CSS+Javascript)功能


3. /task-executor 執行xx/xx/task.md的任務
```



<br><br>




# [instructions](https://github.com/github/awesome-copilot?tab=readme-ov-file#-custom-instructions)




<br><br>


