<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Delete File Issue - Windows Command</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
    }
    .step {
      background-color: #f7f7f7;
      padding: 15px;
      margin: 10px 0;
      border-left: 5px solid #4CAF50;
    }
    pre {
      background-color: #e6e6e6;
      padding: 10px;
    }
    button {
      padding: 10px 20px;
      margin-top: 10px;
      background-color: #4CAF50;
      color: white;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <h1>Solution to "Could Not Find This Item" Error</h1>
  <p>Follow these steps to delete the folder using Command Prompt in Windows.</p>

  <div class="step">
    <h3>Step 1: Open Command Prompt</h3>
    <p>Press <code>Win + R</code>, type <code>cmd</code>, and press Enter to open Command Prompt.</p>
  </div>

  <div class="step">
    <h3>Step 2: Enter the Delete Command</h3>
    <p>Type the following command in the Command Prompt:</p>
    <pre>rd /s "\\?\D:\path-to-folder"</pre>
    <p>Replace <code>D:\path-to-folder</code> with the actual folder location.</p>
    <button onclick="showLocationStep()">Show Example</button>
    <div id="locationExample" style="display:none;">
      <p>For example, if the folder is in the "JAVA 327" directory, the command will be:</p>
      <pre>rd /s "\\?\D:\JAVA 327"</pre>
    </div>
  </div>

  <div class="step">
    <h3>Step 3: Confirm Deletion</h3>
    <p>When prompted with <code>Are you sure (Y/N)?</code>, press <code>Y</code> and hit Enter to confirm.</p>
  </div>

  <div class="step">
    <h3>Step 4: Done!</h3>
    <p>The folder should now be deleted from your system.</p>
  </div>

  <script>
    function showLocationStep() {
      document.getElementById("locationExample").style.display = "block";
    }
  </script>
</body>
</html>
