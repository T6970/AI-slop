<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>Block Code Editor + Preview</title>
<script src="https://unpkg.com/blockly/blockly.min.js"></script>
<style>
  body { margin: 0; font-family: sans-serif; display: flex; height: 100vh; }
  #editor { width: 60%; height: 100%; }
  #preview { width: 40%; height: 100%; border-left: 2px solid #ddd; display: flex; flex-direction: column; }
  iframe { flex: 1; border: none; background: white; }
  #controls { padding: 6px; background: #eee; border-bottom: 1px solid #ccc; }
  button { padding: 6px 10px; }
</style>
</head>
<body>

<div id="editor"></div>

<div id="preview">
  <div id="controls">
    <button onclick="runCode()">Run Code</button>
  </div>
  <iframe id="output"></iframe>
</div>

<script>
  const workspace = Blockly.inject('editor', {
    toolbox: `
    <xml xmlns="https://developers.google.com/blockly/xml">
      <category name="Logic" colour="#5C81A6">
        <block type="controls_if"></block>
        <block type="logic_compare"></block>
      </category>
      <category name="Loops" colour="#5CA65C">
        <block type="controls_repeat_ext">
          <value name="TIMES"><shadow type="math_number"><field name="NUM">10</field></shadow></value>
        </block>
      </category>
      <category name="Math" colour="#5C68A6">
        <block type="math_number"><field name="NUM">0</field></block>
        <block type="math_arithmetic"></block>
      </category>
      <category name="Text" colour="#5CA6A6">
        <block type="text"></block>
        <block type="text_print"></block>
      </category>
      <category name="JS" colour="#AA00AA">
        <block type="text_print"></block>
      </category>
    </xml>
    `
  });

  function runCode() {
    const code = Blockly.JavaScript.workspaceToCode(workspace);
    const iframe = document.getElementById("output");
    iframe.srcdoc = `
      <script>
        let print = (...msg)=>document.body.innerHTML += msg.join(" ") + "<br>";
      </script>
      <script>
        try { ${code} } catch(e){ document.body.innerHTML += "Error: " + e }
      </script>
    `;
  }
</script>

</body>
</html>
