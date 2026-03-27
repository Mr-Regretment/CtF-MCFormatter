# MCFunction NBT Formatter

A simple web-based tool that formats long Minecraft commands (especially NBT data) into clean, readable multi-line `.mcfunction` syntax.

What it does

* Takes messy, single-line Minecraft commands
* Splits and indents NBT structures (`{}` and `[]`)
* Outputs clean, readable formatting
* Optional trailing `\` for multi-line commands

Who it's for

This tool is built for:

* Minecraft **datapack creators**
* Command block users
* Anyone working with **NBT-heavy commands**

Example

### Input

```
/summon zombie ~ ~ ~ {CustomName:"Bob",HandItems:[{id:"minecraft:diamond_sword",Count:1b},{}]}
```

### Output

```
/summon zombie ~ ~ ~ \
{\
  CustomName:"Bob",\
  HandItems:[\
    {\
      id:"minecraft:diamond_sword",\
      Count:1b\
    },\
    {}\
  ]\
}
```

Usage

1. Paste your command into the input box
2. Click **Format**
3. Copy the output into your `.mcfunction` file

Notes

* Formatting is structural, not semantic (it doesn’t validate commands)
* Works best with properly formatted NBT input
---

Live Website
```
https://YOUR-USERNAME.github.io/mcfunction-formatter/
```
