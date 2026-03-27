# Command to Function – MCFunction Multi-Tool

A fast, no-nonsense web tool for transforming messy Minecraft commands into clean, usable `.mcfunction` code.

Built for people who are tired of unreadable NBT.

---

What it does

This tool helps you take long, ugly commands and actually work with them.

### Features

* **Formatter**

  * Converts single-line commands into structured, indented output
  * Handles nested `{}` and `[]` cleanly
  * Makes NBT readable

* **Validator**

  * Checks for broken brackets (`{}`, `[]`)
  * Quickly catches malformed structures

* **Minifier**

  * Compresses commands into compact one-liners
  * Useful for commands or storage

* **Command Splitter**

  * Breaks commands into readable segments
  * Great for debugging or teaching

* **Line Numbers**

  * Makes debugging `.mcfunction` files easier
  * Quickly reference exact lines

---

## Example

### Input

```
/summon zombie ~ ~ ~ {CustomName:"Bob",HandItems:[{id:"minecraft:diamond_sword",Count:1b},{}]}
```

### Output (Formatted)

```
/summon zombie ~ ~ ~
{
  CustomName:"Bob",
  HandItems:[
    {
      id:"minecraft:diamond_sword",
      Count:1b
    },
    {}
  ]
}
```

---

## ⚙️ Usage

1. Paste your command into the input box
2. Select a mode:

   * Format
   * Minify
   * Split
   * Validate
3. Click **Run**
4. Copy the result

---

## Notes

* Formatting is **structural**, not semantic
* It does not validate full Minecraft command syntax
* Best results come from valid NBT input

---

## Live Site

https://mr-regretment.github.io/CtF-MCFormatter/

---

Future Ideas

* NBT syntax highlighting (true parser)
* Error pinpointing (line-level)
* Function file export (multi-command)
* Drag & drop `.mcfunction` support

---

License

Free to use. No nonsense.
