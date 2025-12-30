<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Modular Text Editor</title>
<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    height: 100vh;
  }

  #toolbar {
    background: #333;
    color: white;
    padding: 5px;
    display: flex;
    gap: 5px;
  }

  #toolbar button {
    background: #555;
    color: white;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
  }

  #toolbar button:hover {
    background: #777;
  }

  #editor {
    flex: 1;
    padding: 10px;
    border: none;
    outline: none;
    resize: none;
    font-family: monospace;
    font-size: 16px;
  }
</style>
</head>
<body>

<div id="toolbar">
  <!-- Toolbar buttons will be added by extensions -->
</div>

<textarea id="editor" placeholder="Start typing..."></textarea>

<script>
  // Core editor object
  const Editor = {
    editorEl: document.getElementById('editor'),
    toolbarEl: document.getElementById('toolbar'),
    extensions: [],
    
    registerExtension(extension) {
      this.extensions.push(extension);
      if (extension.init) extension.init(this);
      if (extension.toolbarButton) {
        const btn = document.createElement('button');
        btn.innerText = extension.toolbarButton.label;
        btn.onclick = () => extension.toolbarButton.action(this);
        this.toolbarEl.appendChild(btn);
      }
    },
    
    getText() {
      return this.editorEl.value;
    },
    
    setText(text) {
      this.editorEl.value = text;
    },
    
    insertText(text) {
      const start = this.editorEl.selectionStart;
      const end = this.editorEl.selectionEnd;
      const value = this.editorEl.value;
      this.editorEl.value = value.slice(0, start) + text + value.slice(end);
      this.editorEl.selectionStart = this.editorEl.selectionEnd = start + text.length;
      this.editorEl.focus();
    }
  };

  // Example extensions
  const boldExtension = {
    toolbarButton: {
      label: 'Bold',
      action(editor) {
        const selected = editor.getText().slice(
          editor.editorEl.selectionStart,
          editor.editorEl.selectionEnd
        );
        editor.insertText(`**${selected}**`);
      }
    }
  };

  const helloExtension = {
    toolbarButton: {
      label: 'Hello',
      action(editor) {
        editor.insertText('Hello World!');
      }
    }
  };

  // Register extensions
  Editor.registerExtension(boldExtension);
  Editor.registerExtension(helloExtension);
</script>

</body>
</html>
