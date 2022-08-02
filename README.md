# @docchi/cda-checking

Simple checking package, if cda video is deleted or available.

![Okładka](https://cdn.discordapp.com/attachments/721911008213598238/1001119430358601760/Frame_1_2.png)

## Kontakt

- GitHub: [github.com/ankordii][github]
- Website: [https://docchi.pl/][site]
- E-mail: pomoc@docchi.pl

## Installation

[Node.js](https://nodejs.org/en/) required
```bash
npm install @docchi/cda-checking
```

## How to use

<sub>Don't forget to add
```json
"type": "module"
```
to *package.json*
</sub>

How to use: 

<sub>Examples of ID</sub>
- EMBED URL - **https://ebd.cda.pl/620x395/115890987a**
- VIDEO URL - **https://www.cda.pl/video/115890987a**
- JUST ID - **115890987a**

Example: 

```js
import checkPlayer from "@docchi/cda-checking";

console.log(await 
  checkPlayer("https://www.cda.pl/video/115890987a")
)
```

If available
```json
{
    "status": 200, 
    "message": "Source exists" 
}
```
# Codes

- 500 - Something went wrong!
- 410 - Source removed by administrators.

- 200 - Source exists
- 206 - Page loaded, but couldn't verify if source exists

# Support
<b>IMPORTANT</b>: Help me beeing efficient, please! I am developing in my free time for no money. Contribute to the project by posting complete, structured and helpful issues which I can reproduce quickly without asking for missing information.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/docchi)

# License
[MIT](https://github.com/docchipl/cda-checking/blob/main/LICENSE)

[github]: https://github.com/ankordii
[site]: https://docchi.pl/
