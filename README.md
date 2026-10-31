# Get-Discord-Token

Simple browser bookmark to get your Discord token.

## Setup
1. Create a bookmark on any page.
2. Right-click → Edit.
3. Paste the javascript code below into the URL field:
4. Save it
```js
javascript:(function()%7Bvar d%3Dfalse%3Bvar o%3DXMLHttpRequest.prototype.setRequestHeader%3BXMLHttpRequest.prototype.setRequestHeader%3Dfunction(k%2Cv)%7Bif(!d%26%26String(k).toLowerCase()%3D%3D%3D'authorization')%7Bd%3Dtrue%3BXMLHttpRequest.prototype.setRequestHeader%3Do%3Btry%7Bnavigator.clipboard.writeText(v)%7Dcatch(e)%7B%7Dprompt('Your Discord token (copied if your browser allows it)%3A'%2Cv)%7Dreturn o.apply(this%2Carguments)%7D%3Balert('Now click around in Discord (open a server%2C send a message) — your token will pop up.')%7D)()%3B
```
## Usage
1. Open Discord in your browser.
2. Click the bookmark.
3. Click anywhere in Discord (channel, server, etc.).
4. Token appears and is able to be copied.

**Adding image examples soon**
