# proact - a react ripoff...

### Example use case:

```javascript
const someDeepChild = {
    type: 'div',
    classes: ['container'],
    children: [
        {
            type: 'p',
            classes: ['some-text']
        }
    ]
};
const someProactApp = {
    {
        type: 'div',
        children: [
            {
                type: 'p',
                text: 'hello',
                classes: ['big-text', ''],
            },
            {
                type: 'div',
                children: [
                    someDeepChild
                ]
            }
        ]
    },
};

Proact.render(someProactApp, document.getElementById('root'))
```
