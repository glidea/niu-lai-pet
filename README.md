# 牛来 Codex Pet

牛来是一个 Codex v2 动态宠物，包含 9 行标准动作和 16 个顺时针视线方向。

## 安装

```bash
mkdir -p ~/.codex/pets/niu-lai
cp pet.json spritesheet.webp ~/.codex/pets/niu-lai/
```

重启 Codex 后即可使用。安装目标文件为：

```text
~/.codex/pets/niu-lai/pet.json
~/.codex/pets/niu-lai/spritesheet.webp
```

## 校验

```bash
jq '.spriteVersionNumber' ~/.codex/pets/niu-lai/pet.json
```

输出应为 `2`。精灵图尺寸为 `1536x2288`，单帧尺寸为 `192x208`。

`qa/` 保存最终校验结果，`assets/` 保存两行视线源图和四方向锚点。
