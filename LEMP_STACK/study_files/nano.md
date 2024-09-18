# Nano Editor Documentation and Basic Commands

**Nano** is a versatile and user-friendly text editor available on most Unix-based systems. It is well-suited for both beginners and experienced users, offering an intuitive interface and essential editing functionalities. Unlike more complex editors such as Vim or Emacs, Nano provides a smoother learning curve, making it ideal for quick text edits and basic manipulations.

## Opening Files

To edit an existing file or create a new one, use the following command in the terminal:

```
nano henryfile.txt
```

Replace `henryfile` with the actual name of the file you want to open. If the file does not exist, Nano will create a new file with the given name.

![Opening File in Nano](./images/nano-open-file.png)

## Saving Changes

After making changes to your file, save your work by pressing:

```
Ctrl + O
```

A prompt will appear asking you to confirm the filename. Press `Enter` to keep the existing name, or type a new name followed by `Enter` to save under a different name.

![Saving Changes in Nano](./images/nano-save-changes.png)

## Exiting Nano

To exit Nano, press:

```
Ctrl + X
```

If you have unsaved changes, Nano will prompt you to confirm if you want to save them before closing.

![Exiting Nano](./images/nano-exit.png)

## Basic Navigation

- **Cursor Movement:** Use the arrow keys (`Up`, `Down`, `Left`, `Right`) to navigate through the text.
- **Page Scrolling:** Move down a page with `Ctrl + V` and up a page with `Ctrl + Y`.


## Editing Text

- **Inserting Text:** Start typing at the desired location in the file to add new text.
- **Deleting Text:** Use the `Backspace` or `Delete` key to remove characters.

**Note:** Nano does not have built-in cut, copy, and paste functionalities like some other editors. However, you can use terminal commands or mouse actions to perform these operations.


## Searching for Text

To search for specific text within the file, press:

```
Ctrl + W
```

Enter the text you want to find and press `Enter` to begin the search.

![Searching for Text in Nano](./images/nano-search.png)

## Additional Considerations

- **Undo:** Nano does not have a comprehensive undo feature, but you can undo the most recent action with the `Alt + U` shortcut.
- **Redo:** Nano currently does not support a built-in redo functionality.

![Undo and Redo in Nano](./images/nano-undo-redo.png)

## Conclusion

Nano is a powerful and straightforward text editor that provides essential text editing capabilities within the terminal environment. Its user-friendly interface and basic commands make it an excellent tool for both new and experienced users. As you become more familiar with Nano, you may discover additional features and shortcuts to enhance your editing experience.

![Overview of Nano](./images/nano-overview.png)

For further learning, you can explore more about Nano through its [official documentation](https://nano-editor.org/docs.php).
