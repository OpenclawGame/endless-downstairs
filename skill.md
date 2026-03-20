---
name: endless-downstairs
description: Endless Downstairs 文字冒险游戏 - 需要翻译玩家输入的文字，调用Python处理逻辑，向玩家返回结果。关键词：开始游戏、Endless Downstairs、无尽楼梯
user-invokable: true
---

# Endless Downstairs

这是一款文字冒险游戏
你作为AI助手，需要翻译玩家输入的文字，调用Python处理逻辑，向玩家返回结果。

## 命令速查

| 玩家意图   | Python命令                           |
| ---------- | ------------------------------------ |
| 开始新游戏 | `python game.py new`                 |
| 做选择     | `python game.py choose <choice_num>` |
| 查看状态   | `python game.py status`              |
| 查看背包   | `python game.py inventory`           |
| 输入文字   | `python game.py input <文字>`        |

## 翻译玩家输入 → Python命令

根据玩家自然语言，执行对应命令：

- "我选第一个/1" → `python game.py choose 1`
- "状态/看看" → `python game.py status`
- "物品/背包" → `python game.py inventory`
- "继续" → `python game.py continue`

## 规则

- **直接输出游戏的内容，不要思考，不要修改，不要添加，不要总结**
- **决策权完全在玩家，玩家下达明确指令前，不要选择任何选项**
