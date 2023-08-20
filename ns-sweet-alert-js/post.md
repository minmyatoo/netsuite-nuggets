## Using Sweet Alert JS in a NetSuite User Event Script

To incorporate Sweet Alert JS into a NetSuite User Event Script, you can follow the code examples below:

### Sweet Alert Script

```javascript
swal("Hello Myatkrub!");
```

### UserEvent Script SS1.0

```javascript
function beforeLoad(type, form, request) {
    if (type == 'create') {
        var sweet = '';
        sweet += '<html><body><script src="https://unpkg.com/sweetalert/dist/sweetalert.min.js"></script><script type=\'text/javascript\'>swal("Hello Myatkrub!")</script></body></html>';
        var field = form.addField("custpage_alertfield", "inlinehtml");
        field.setDefaultValue(sweet);
    }
}
```

You can also explore and integrate other types of alerts and pop-ups from [Sweet Alert's website](https://sweetalert.js.org/) for more options.
```

This Markdown format should render your text with appropriate headings and code blocks.
