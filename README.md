# TagUI Cheat Sheet

<a href="https://github.com/aisingapore/TagUI/releases/tag/v6.110.0" alt="For TagUI version v6.110">
        <img src="https://img.shields.io/badge/for%20TagUI%20version-v6.110-blue" />
</a>
<a href="https://github.com/chuamatt/tagui-cheatsheet/pulls">
        <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" />
</a>


### Basics
- TagUI auto-waits for a webpage element to appear and interacts with it as soon as it appears
- Element identifier can be auto-recorded using TagUI Chrome extension, or [found from web browser](https://tagui.readthedocs.io/en/latest/faq.html#element-attributes)
- Identifiers help to pinpoint which webpage elements you want to interact with ([examples in flow samples](https://github.com/aisingapore/TagUI-Bricks))
- TagUI auto-selects provided identifier in this order - XPath, CSS, id, name, class, title, aria-label, text(), href

<div class="tg-wrap"><table><thead><tr><th style="text-align:left">Mouse and Keyboard</th><th style="text-align:left">Parameters (separator in bold)</th><th style="text-align:left">Purpose</th><th style="text-align:left">Example</th></tr></thead><tbody><tr><td>http(s)://</td><td>[URL]</td><td>go to specified webpage</td><td>https://google.com</td></tr><tr><td>click</td><td>click [DOM/XPath/Point/Image]</td><td>left-click on an identifier</td><td rowspan="4">click Main concepts<br>rclick //nav/div[2]/a<br>dclick (500,200)<br>hover button.png</td></tr><tr><td>rclick</td><td>rclick [DOM/XPath/Point/Image]</td><td>right-click on an identifier</td></tr><tr><td>dclick</td><td>dclick [DOM/XPath/Point/Image]</td><td>double-click on an identifier</td></tr><tr><td>hover</td><td>hover [DOM/XPath/Point/Image]</td><td>move cursor to identifier</td></tr><tr><td>type</td><td>type [DOM/XPath/Point/Image] <strong><em>as</strong></em> [text] ([enter] = enter, [clear] = clear field)</td><td>enter element as text</td><td>type search-term as John Wick<br>type //input[@name="search"] as John Wick<br>type (500,200) as [clear]John Wick[enter]<br>type input_field.png as John Wick</td></tr><tr><td>keyboard</td><td>keys to click</td><td>enter keystrokes directly</td><td>keyboard [win]run[enter]<br>keyboard [printscreen]<br>keyboard [ctrl]c</td></tr><tr><td>mouse</td><td>down/ up</td><td>sends a mouse event at current position</td><td>mouse up<br>mouse down</td></tr></tbody></table></div>

# Acknowledgements

The original source for this cheat sheet can be found [here](https://github.com/aisingapore/TagUI/tree/pre_v6#cheat-sheet), licensed under the Apache 2.0 license. I have added some additional information to the original cheat sheet to make it more comprehensive and  keep it up to date. I've also made some minor formatting modifications to make it more readable and easier to understand.