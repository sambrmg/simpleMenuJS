# Simple Menu JS

This is a menu in javascript to simplify your project when you need a dynamic menu. Just put Json with this structure.  

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
