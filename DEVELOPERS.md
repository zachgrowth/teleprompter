TelePrompter - Developer Setup
--

> Want to run this on your own server? Here is all you need to do:

![icon](assets/img/icon-256x256.png "icon")

#### Clone Repo

```bash
git clone git@github.com:manifestinteractive/teleprompter.git
cd teleprompter
npm install
```

#### Start Application

```bash
npm start
```

Automated Control
---

If you are feeling super fiesty, you can control the TelePrompter using the following Client Side Javascript:

```js
// Initialize TelePrompter ( happens on Page Load)
TelePrompter.init()

// Get Current Configuration for everything, or a specific property
TelePrompter.getConfig()
TelePrompter.getConfig('fontSize')

// Reset TelePrompter
TelePrompter.reset()

// Turn Dim On or Off
TelePrompter.setDim(true)
TelePrompter.setDim(false)

// Turn Flip X On or Off
TelePrompter.setFlipX(true)
TelePrompter.setFlipX(false)

// Turn Flip Y On or Off
TelePrompter.setFlipY(true)
TelePrompter.setFlipY(false)

// Set Font Size
TelePrompter.setFontSize(60)

// Set Page Speed
TelePrompter.setSpeed(30)

// Start TelePrompter
TelePrompter.start()

// Stop TelePrompter
TelePrompter.stop()

// Chain together commands
TelePrompter.setSpeed(30).setFontSize(60).start()

// Get Version Number
TelePrompter.version

// Enable / Disable Debugging ( `false` by default )
TelePrompter.setDebug(true)
TelePrompter.setDebug(false)
```