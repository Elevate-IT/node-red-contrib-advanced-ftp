# node-red-contrib-advanced-ftp

A Node-RED node for advanced FTP operations, with extended runtime control and logging capabilities.

> 🛠️ Forked and maintained by [Elevate IT](https://github.com/Elevate-IT), based on the original work by [anversoft](https://github.com/anversoft/node-red-contrib-advanced-ftp).

[![NPM](https://nodei.co/npm/node-red-contrib-advanced-ftp.png)](https://www.npmjs.com/package/node-red-contrib-advanced-ftp)

---

## ✨ What's New in This Fork?

This fork introduces a new operation:

### ✅ `PUTRENAME`

A convenient one-step action that first uploads a file (`PUT`) and immediately renames it on the server (`RENAME`). This is especially useful for workflows where you want to avoid processing partially uploaded files on the server.

---

## 📦 Installation

### Using npm:

Run the following in your Node-RED user directory (usually `~/.node-red`):

```bash
npm install node-red-contrib-advanced-ftp
```

Then restart Node-RED.

### Using the Node-RED Palette:

- Open Node-RED
- Go to **Menu → Manage palette → Install**
- Search for `node-red-contrib-advanced-ftp` and install

---

## ⚙️ Usage

The node supports a variety of FTP operations. These can be set either statically in the editor or dynamically at runtime via `msg.operation`.

### Supported operations:

- `status`
- `pwd`
- `system`
- `list`
- `get`
- `put`
- `append`
- `rename`
- `delete`
- `mkdir`
- `rmdir`
- ✅ `putrename` ← *New!*

You can modify paths, filenames, and other parameters dynamically via `msg` properties.

---

## 🧪 Example Flow

Here's an example of how to use the FTP Client node to perform different FTP operations dynamically:

<details>
<summary>Click to expand example flow JSON</summary>

```json
[PASTE FULL EXAMPLE FLOW JSON HERE]
```

</details>

---

## 🔒 FTP Logger

Also included is an FTP Logger node that periodically logs data to files, rotates them, and uploads to an FTP server.

---

## 🙌 Acknowledgements

This project uses the following libraries:

- [node-ftp](https://github.com/mscdex/node-ftp) – Asynchronous FTP client for Node.js.
- [fs-extra](https://github.com/jprichardson/node-fs-extra) – File system utilities with promise support and enhancements.

---

## 📄 License

Apache License 2.0 – See [LICENSE](https://github.com/Elevate-IT/node-red-contrib-advanced-ftp/blob/main/LICENSE).

---

## 🤝 Contributing

We welcome issues and pull requests!  
Open an issue or PR at: [https://github.com/Elevate-IT/node-red-contrib-advanced-ftp/issues](https://github.com/Elevate-IT/node-red-contrib-advanced-ftp/issues)

---

## 👥 Contributors

Thanks to all contributors past and present!

Original project:  
[![Contributors](https://contrib.rocks/image?repo=anversoft/node-red-contrib-advanced-ftp)](https://github.com/anversoft/node-red-contrib-advanced-ftp/graphs/contributors)

Fork maintained by: [Elevate IT](https://github.com/Elevate-IT)