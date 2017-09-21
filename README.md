# Simple Menu JS

This is a menu in javascript to simplify your project when you need a dynamic menu. Just put Json with this structure.  

## How to use

Just put `<nav class="simple-menu-js"></nav>` in your html after `body` tag.
To initialize menu you need to call `this.simpleMenuJSinit(jsonMenu)` and pass by parameter Json Object Menu.

## HTML Structure
```html
<ul>
    <li>
        <a href="" class="icon-minus">Google</a>
        <ul>
            <li>
                <a href="https://www.google.com.br/maps/">Maps</a>
            </li>
            <li>
                <a href="#" class="icon-minus">My Account</a>
                <ul>
                    <li>
                        <a href="https://myaccount.google.com/security">Security</a>
                    </li>
                    <li>
                        <a href="https://myaccount.google.com/privacy">Privacy</a>
                    </li>
                </ul>
            </li>
        </ul>
    </li>
</ul>
```

## Json Structure 
Json structure to mount the menu.

You need `label`, `href` and `n` if has child, if has no child don't put index `n` like this `{ "label": "item 2", "href": "#" }`
If `href` is not link or route put only `"href": "#"` or `"href": ""`

```json
[
    { 
        "label": "item 1", 
        "href": " ",
        "n": [
            {
                "label":"subitem 1", 
                "href": "#",
                "n": [{
                    "label":"Google",
                    "href": "http://www.google.com.br"
                }]
            },{
                "label":"subitem 2", 
                "href": "#",
                "n": [{
                    "label":"sub-subitem 2.1",
                    "href": "#"
                },
                {
                    "label":"sub-subitem 2.2",
                    "href": "#"
                }]
            }
        ]
    },
    { "label": "item 2", "href": "#" },
    { "label": "item 3", "href": "#" }
]
```

## Screenshot

<div style="text-align:center">
	<img src="https://sambrmg.github.io/simpleMenuJS/docs/simpleMenuJS.png" alt="simple menu js">
</div>
