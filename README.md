# Corne Keyboard Custom Keymap

A highly optimized ZMK keymap configuration for Corne (crkbd) 3x6 split keyboard, designed specifically for developers and Vim users working with BSPWM window manager.

![c50aa73b6f42e01cb953](https://github.com/user-attachments/assets/23f9bb6e-1d88-4833-ad0e-c419bd37f5ac)


## ✨ Features

- **Vim-Optimized Navigation**: HJKL arrow keys and ESC/CTRL combo key
- **Developer-Friendly Symbol Layer**: Logical grouping of brackets and operators
- **RGB Underglow Support**: 54 LEDs (27 per side)
- **Bluetooth Connectivity**: Support for multiple BT profiles
- **Conditional Layer Activation**: Automatic layer 3 access when holding both layer keys

## 🎹 Keyboard Layout

### Layer 0: Default (QWERTY)

```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│ TAB │  Q  │  W  │  E  │  R  │  T  │       │  Y  │  U  │  I  │  O  │  P  │BSPC │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│SHFT │  A  │  S  │  D  │  F  │  G  │       │  H  │  J  │  K  │  L  │  ;  │  '  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│CT/ES│  Z  │  X  │  C  │  V  │  B  │       │  N  │  M  │  ,  │  .  │  /  │ ESC │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ GUI │LOWER│ SPC │       │ ENT │RAISE│ ALT │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Special Keys:**
- **Left Shift Position**: Tap once for Shift, tap twice for Caps Lock
- **Left Ctrl Position (CT/ES)**: Tap for ESC, hold for CTRL (perfect for Vim users)
- **Left Thumb (GUI)**: Windows/Super key for BSPWM window management

### Layer 1: Lower (Numbers & Navigation)

```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │  1  │  2  │  3  │  4  │  5  │       │  6  │  7  │  8  │  9  │  0  │ DEL │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │     │       │  ←  │  ↓  │  ↑  │  →  │     │PG UP│
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │ ⌘Z │ ⌘X │ ⌘C │ ⌘V │     │       │HOME │ END │     │     │     │PG DN│
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │     │       │     │     │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Features:**
- Number row on left hand (1-5) and right hand (6-0)
- Vim-style arrow keys (HJKL → ←↓↑→)
- Text editing shortcuts (Undo, Cut, Copy, Paste)
- Page navigation (Home, End, PgUp, PgDn)

### Layer 2: Raise (Symbols)

```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│  `  │  !  │  @  │  #  │  $  │  %  │       │  ^  │  &  │  *  │  (  │  )  │BSPC │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │     │       │  -  │  =  │  [  │  ]  │  \  │  |  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │     │       │  _  │  +  │  {  │  }  │  ~  │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │     │       │     │     │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Optimized for Coding:**
- Matching brackets grouped together: `()`, `[]`, `{}`
- Math operators: `-`, `=`, `+`, `_`
- Special symbols easily accessible

### Layer 3: Adjust (System)

```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│ F1  │ F2  │ F3  │ F4  │ F5  │ F6  │       │ F7  │ F8  │ F9  │ F10 │ F11 │ F12 │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│BTCLR│ BT0 │ BT1 │ BT2 │ BT3 │ BT4 │       │OUTTG│ BR+ │ BR- │ EF+ │ EF- │RGBTG│
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│EPTOG│     │     │     │     │     │       │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │     │       │     │     │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Access**: Hold both **LOWER** and **RAISE** simultaneously

**System Controls:**
- **F1-F12**: Function keys
- **BTCLR**: Clear all Bluetooth pairings
- **BT0-BT4**: Select Bluetooth profile (0-4)
- **OUTTG**: Toggle output between USB and Bluetooth
- **BR+/BR-**: RGB brightness increase/decrease
- **EF+/EF-**: RGB effect next/previous
- **RGBTG**: Toggle RGB on/off
- **EPTOG**: Toggle external power

## 🔧 Hardware Components

### RGB Underglow
- **Total LEDs**: 54 (27 per side)
- **LED Types**: 
  - 6× WS2812B per side
  - 21× SK6812 Mini-E per side
- **Chain Length**: 27 LEDs per half

### Required Hardware
- Corne (crkbd) PCB with 3x6 layout
- Pro Micro compatible controller (Nice!Nano or NRF52840 recommended for wireless)
- RGB LED strips (WS2812B/SK6812)
- Key switches (MX or Choc compatible)
- TRRS cable (for wired split) or wireless modules
- Battery 20000mah : 2
- Case : [Corn_Case](https://drive.google.com/drive/folders/19AkEc42lhCGgMnnU6OsV1ynqd6RLx59a?usp=sharing)

## 📦 Installation
1. Download and extract the [Corne Firmware](https://github.com/thien0709/corne_config/releases/tag/Firmware_Corne)
2. **Enter Bootloader:**
   Connect the keyboard to your PC via USB. Quickly **double-tap the Reset button**. A storage drive named `NICENANO` will appear on your computer.
3. **Flash Firmware:**
   Drag and drop the corresponding `.uf2` file into the `NICENANO` drive.
   * Use the `corne_left nice_oled-nice_nano_v2-zmk.uf2` file for the **Left** keyboard.
   * Use the `corne_right nice_oled-nice_nano_v2-zmk.uf2` file for the **Right** keyboard.
   *(The drive will automatically close, and the keyboard will reboot when finished).*
4. **Sync (Pairing):**
   After flashing both sides, unplug the USB. Turn on battery power for both halves. Press the **Reset button once on both sides** at the same time to let them pair wirelessly.

## 📚 Resources

- [ZMK Documentation](https://zmk.dev/docs)
- [ZMK Key Codes](https://zmk.dev/docs/codes)
- [Corne Keyboard Guide](https://github.com/foostan/crkbd)

## 📄 License
This keymap configuration is provided as-is for personal use and modification.

**Happy Typing! ⌨️**
