# Markdown Example

## Basic Elements

### 段落

段落のテスト。
複数行の文章であっても同一段落として変換される。

空行によって新しい段落として扱われる。

**強調**表示や*斜体*の確認。

### 箇条書き

- ひとつ
- ふたつ
- みっつ
  - one
  - two
  - three

1. Time
2. Minute
3. Second

### 図

図画の挿入。

#### SVGの場合

![SVG Hex Tile Figure](./figs/hex.svg "Hex")

#### PNGの場合

画像フォーマットによって Pandoc が生成するタグが変わるかもしれない。

![GitHub ICON by PNG](./figs/github-icon.png "GitHub ICON")

draw.io の Web ICON パッケージに GitHub ICON が存在する。

### 表

#### Ubuntu LTS Version's Code Name

|Version|Name|
|:--:|:--:|
| 16.04 | Xenial Xerus |
| 18.04 | Bionic Beaver |
| 20.04 | Focal Fossa |
| 22.04 | Jammy Jellyfish |

#### 無次元のスケール

|呼び名| スケール|
|:--|--:|
|ミリ| 1/1000|
|センチ| 1/100|
|デシ| 1/10|
|デカ| 10|
|ヘクト| 100|
|キロ| 1000|

## リンク

[このリポジトリ](https://github.com/lotcarnage/pandoc-markdown-to-html-template)

## Programing code

### C言語

```c
/* C言語のソースコード */
#include <stdio.h>
#include <stdint.h>

typedef union IPv4Address_ {
    uint32_t value;
    uint8_t octets[4];
} IPv4Address;

static const IPv4Address s_localhost_address = {
    .octets= {127, 0, 0, 1}
};

extern const volatile uint32_t* memory_mapped_io_register;

int main(void)
{
    printf("%lu\n", sizeof(s_localhost_address));
    for (;;) {
        if (*memory_mapped_io_register != 0u) {
            break;
        }
    }
    return 0;
}
```

### Python

```python
#!/usr/bin/env python3
import numpy

def _main() -> None:
    print('hello')
    return None

if __name__ == "__main__":
    _main()
    exit()
```
