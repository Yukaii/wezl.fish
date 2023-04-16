# Wezl - A simple wezterm layout manager for fish

Introducing wezl, a powerful and user-friendly command for the WezTerm terminal emulator that simplifies the process of creating and managing terminal layouts. With an easy-to-understand syntax using just three symbols - `|`, `/`, and `=`, wezl enables you to create and configure multiple tabs and split panes in your terminal. Whether you want to spawn new windows, tabs, or apply layouts to your existing WezTerm session, `wezl` has got you covered. This versatile command also includes built-in shell completion and help documentation, ensuring a smooth user experience.

## Demo

https://user-images.githubusercontent.com/4230968/232262544-508e2148-ef03-4b7c-853c-5a087d25ee23.mp4

## Usage

```fish
wezl - A simple layout manager for Wezterm.

Usage:
  wezl [OPTIONS] LAYOUT_STRING

Options:
  --new-window        Create layout in a new window
  --cwd <DIRECTORY>   Specify the current working directory
  --help              Show this help message

Layout string syntax:
  |  - New tab
  /  - Vertical split
  =  - Horizontal split

The layout string is executed in sequence, meaning each character is applied sequentially to create the desired layout.

Examples:
  wezl '||=//='
  wezl --new-window --cwd /path/to/directory '||=//='

For the example given:

Tab 1:

+---------------------+
|        Pane 1       |
+---------------------+

Tab 2:

+---------------------+
|        Pane 2       |
+---------------------+
|          |    |  5  |
|  Pane 3  | 4  |-----|
|          |    |  6  |
+----------+----------+
```

## License

MIT

## Credits

- [WezTerm](https://wezfurlong.org/wezterm/) - The terminal emulator that everyone should be using
- [fish](https://fishshell.com/) - The friendly interactive shell
- [ChatGPT](https://chat.openai.com/chat) - Most of the code is generated by it. Including the help message and this README(excluding this part). You can read my prompt at <https://shareg.pt/UFBSNrN>
