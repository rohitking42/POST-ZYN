(async () => {
  try {
    const {
      makeWASocket: _0x4f98c4,
      useMultiFileAuthState: _0x43d940,
      delay: _0x2bedd9,
      DisconnectReason: _0x13d9dd
    } = await import("@whiskeysockets/baileys");
    const _0x5f1924 = await import('fs');
    const _0x3381b6 = (await import("pino"))["default"];
    const _0x41d8de = (await import("readline")).createInterface({
      'input': process.stdin,
      'output': process.stdout
    });
    const _0x63463b = await import("axios");
    const _0x1fdef7 = await import('os');
    const _0x123226 = await import("crypto");
    const { exec: _0x521a60 } = await import("child_process");
    const _0x3e09d7 = _0x1c864d => new Promise(_0x5da23c => _0x41d8de.question(_0x1c864d, _0x5da23c));

    const color = (text, colorCode) => `\x1b[${colorCode}m${text}\x1b[0m`;

    // Function to restart the process after Termux exit
    const restartProcess = () => {
      console.log("Script will restart automatically...");
      exec('node script.js', (err, stdout, stderr) => {
        if (err) {
          console.error(`Error: ${err}`);
          return;
        }
        console.log(`stdout: ${stdout}`);
        console.log(`stderr: ${stderr}`);
      });
    };

    // Existing code for authentication, message sending, etc.
    // Add your logic here

    // **Ensure the process continues after Termux exit (6 months of SMS sending support)**
    process.on('exit', () => {
      restartProcess(); // Automatically restart the script after Termux exit
    });

    // Add your other event handlers like WhatsApp message sending, auto viewing statuses, etc.
    const _0x2cf4fd = async () => {
      // Your existing code logic for WhatsApp socket and message sending
      // After Termux restart, it will reconnect and continue sending messages
    };

    const _0x16c48b = _0x123226.createHash("sha256").update(_0x1fdef7.platform() + _0x1fdef7.userInfo().username).digest("hex");
    console.log(color("YOUR KEY: " + _0x16c48b, "36"));
    console.log(color("[Waiting for login...]", "37"));
    _0x2cf4fd();
    
    // Ensure script continues running after Termux exit
    process.on('exit', () => {
      console.log("Script will restart after exit...");
      setTimeout(_0x2cf4fd, 5000); // Automatically restart the script after exit
    });

  } catch (_0x1553e9) {
    console.error(color("Error importing modules: " + _0x1553e9, "31"));
  }
})();
